# Method

The CO2 values presented here compare mass-timber projects with reference construction using concrete, steel, or other conventional materials. The dataset uses three approaches: project-specific results reported in published sources, screening estimates based on timber volume, and a whole-building life-cycle assessment calculation for Marpole Community Centre.

The CO2 benefit includes two quantities where both are available:

- **Avoided emissions:** estimated emissions avoided when wood is used in place of more emissions-intensive materials such as concrete or steel.
- **Stored carbon:** atmospheric CO2 absorbed during tree growth and retained as biogenic carbon in wood products.

Where a published source provides only a combined total, the dataset reports that total without assigning separate avoided-emissions and stored-carbon values.

## 1. Published project results

Seven of the 11 projects use carbon results reported in project-specific published sources.

- **Brock Commons Tallwood House**  
  https://sustain.ubc.ca/sites/default/files/brock_commons_storyboards_0.pdf

- **UBC Earth Sciences Building**  
  https://www.arataumodular.com/app/wp-content/uploads/2022/06/Cross-Laminated-Timber-Taking-wood-buildings-to-the-next-level.pdf

- **UBC Centre for Interactive Research on Sustainability**  
  https://www.naturallywood.com/wp-content/uploads/centre-for-interactive-research-on-sustainability_case-study_naturallywood.pdf

- **Vancouver Convention Centre West Building**  
  https://www.naturallywood.com/wp-content/uploads/vancouver-convention-centre-west-building-case-study-oct2010-naturallywood.pdf

- **Richmond Olympic Oval**  
  https://www.naturallywood.com/wp-content/uploads/richmond-olympic-oval-case-study-oct2010-naturallywood.pdf

- **The Hive**  
  https://dialogdesign.ca/news-events/canadas-greenest-employers-2026-five-dialog-projects-moving-sustainable-design-forward/

- **oN5 Building**  
  https://westvancouver.ca/sites/default/files/media/documents/22jul06.pdf

## 2. Timber-volume screening estimates

Three projects—BCIT Tall Timber Student Housing, the Freedom Mobile Arch, and the SFU Stadium Mass-Timber Canopy—use timber-volume-based screening estimates because a project-specific published CO2 total was not identified in the sources reviewed.

The calculations use factors documented by the WoodWorks Carbon Calculator:

- **Calculator:**  
  https://cc.woodworks.org/carbon-calculator

- **References and calculation notes:**  
  https://cc.woodworks.org/pdf/2025_carbon_calculator_references_notes.pdf

### Wood mass

Timber volume is first converted to oven-dry wood mass:

**Dry wood mass = timber volume × oven-dry wood density**

The calculations use an oven-dry density of **446 kg/m³**, equivalent to **0.446 metric tonnes/m³**.

This density is taken from the Kalesnikoff CLT Environmental Product Declaration:

https://kalesnikoff.com/wp-content/uploads/2022/05/Kalesnikoff-CLT-EPD-.pdf

### Avoided emissions

The WoodWorks methodology uses a mass-timber displacement factor of **0.71 tonnes of avoided CO2-equivalent per metric tonne of oven-dry wood**:

**Avoided emissions = dry wood mass × 0.71**

Using a density of 0.446 t/m³:

**Avoided emissions = timber volume × 0.317 tCO2e/m³**

For the screening calculations in this dataset, a coefficient of **0.31 tCO2e/m³** is used.

### Stored carbon

Stored carbon is calculated by assuming that carbon accounts for 50% of oven-dry wood mass and converting the carbon mass to its CO2 equivalent using the molecular-weight ratio 44/12:

**Stored carbon = dry wood mass × 0.50 × 44/12**

This is equivalent to:

**Stored carbon = dry wood mass × 1.833**

Using a density of 0.446 t/m³:

**Stored carbon = timber volume × 0.818 tCO2/m³**

For the screening calculations in this dataset, this is expressed as **0.82 tCO2/m³**.

### Project inputs

#### BCIT Tall Timber Student Housing

The calculation uses a CLT volume of **2,289.117 m³**, extracted from the public Fast + Epp Revit model available through Speckle.

- https://app.speckle.systems/projects/723ddc61a3/models/5a36c2c7dc
- https://www.fastepp.com/portfolio/bcit-student-housing/

#### Freedom Mobile Arch

Published project information states that the structure contains **more than 2,000 m³ of mass timber**. The calculation uses **2,000 m³** as the input volume.

- https://construireenboisvol17no1en.cecobois.com/integrating-embedded-carbon-in-design-choices/low-carbon-projects
- https://reveryarchitecture.com/projects/pne-amphitheatre/

#### SFU Stadium Mass-Timber Canopy

The calculation uses an estimated CLT volume of **179.731 m³**:

**941 m² × 0.191 m = 179.731 m³**

The canopy area of 941 m² is published project information. The **191 mm thickness is inferred from the specified seven-ply CLT configuration**.

- https://sfss.ca/wp-content/uploads/2017/10/Board-Of-Directors-2017-09-29.pdf
- https://perkinswill.com/getting-to-craft-in-mass-timber-design/
- https://cwc.ca/wp-content/uploads/2025/08/Structurlam-Canadian-Mass-Timber-Technical-Guide-June-2020.pdf

## 3. Marpole Community Centre

Marpole Community Centre uses a whole-building life-cycle assessment calculation.

The published project information reports:

- **Conventional baseline:** 605 kgCO2e/m²
- **Proposed building:** 362 kgCO2e/m²
- **Building area:** 6,100 m²

The CO2e reduction is calculated as:

**CO2e reduction = (605 − 362) × 6,100 ÷ 1,000**

**= 1,482.3 tCO2e**

The dataset reports this as **1,482 tCO2e**.

The available documentation treats biogenic carbon separately and does not provide a project-level stored-carbon total, so no separate stored-carbon value is entered.

https://clfbritishcolumbia.com/marpole-community-centre/

## 4. Tree-equivalent illustration

The tree-equivalent figure uses an assumed absorption rate of **22 kg of CO2 per tree per year over 50 years**.

Under this assumption:

**22 kg CO2/year × 50 years = 1,100 kg CO2 = 1.1 tonnes CO2 per tree**

The tree equivalent is calculated as:

**Equivalent trees = total CO2 benefit ÷ 1.1**