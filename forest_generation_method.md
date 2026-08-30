# How the forest map is created

The map starts with a project location and a required number of trees. Tree locations are formed as a Matérn cluster pattern: loose groups are established at random, then trees are scattered around each group. Groups can overlap or remain separate, producing a mixture of denser stands, isolated trees, and open gaps.

This initial pattern is overlaid on OpenStreetMap data downloaded using Overpass Turbo. Permitted ground begins as the circular search area around the project, clipped to the land side of any `natural=coastline`. The following mapped features are removed:

- `building=*`
- `highway=*`
- `railway=*`
- `waterway=*`, including `waterway=riverbank` relations
- `aeroway=*`
- `power=substation`
- `landuse=industrial`, `construction`, `farmland`, `farmyard`, `military`, `quarry`, `landfill`, `cemetery`, or `reservoir`
- `amenity=grave_yard`
- `leisure=pitch`, `playground`, `schoolyard`, `swimming_pool`, or `golf_course`
- `natural=water`, `wetland`, `bay`, `beach`, `sand`, or `scree`

Spatial geometry operations are performed with the Shapely Python library.

Road and path exclusions use the mapped width when available, otherwise an estimated width based on lanes or highway type. Roadside planting strips are identified beside `highway=secondary`, `tertiary`, `unclassified`, `residential`, `living_street`, and `service`, while remaining subject to the other exclusions. For the oN5 Building, the only project-specific rule is that `highway=footway` is not used as an exclusion. All other generation rules remain unchanged.

Everything left in the land mask is permitted, including `landuse=residential`, `amenity=parking`, `amenity=bicycle_parking`, `amenity=bicycle_rental`, `natural=wood`, `leisure=park`, mapped trees, and unmapped open ground. The search begins around the project and extends outward only until the required number of valid tree locations is found.

The final tree locations define the forest-area layer. A concave outline follows the irregular form of each tree cluster. The outline is expanded slightly to represent the surrounding stand, then trimmed where it meets the same restricted map features.

## Reference for the clustered tree pattern

Lutz, J. A., Larson, A. J., Freund, J. A., Swanson, M. E., and Bible, K. J. (2013). “The Importance of Large-Diameter Trees to Forest Structural Heterogeneity.” *PLOS ONE* 8(12): e82784. The study used a Matérn cluster process to simulate aggregated tree patterns in mapped temperate forests.

https://doi.org/10.1371/journal.pone.0082784
