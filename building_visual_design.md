# 3D building visual design

The 3D elements and custom shaders are built on the deck.gl framework. The building layer uses color, form, and screen-space effects to give the city a lively character and keep individual buildings visually clear.

## Color variation

Each building receives a random color from a coordinated palette. The variation reflects the visual diversity of a city and helps distinguish neighboring buildings.

## Rounded form

Building corners are softly rounded. This creates a gentler overall appearance and separates adjacent building forms more clearly.

## Orthographic projection

An orthographic view reduces perspective distortion and keeps building forms visually consistent across the scene.

## Lighting

Soft ambient and directional lighting shapes the building surfaces and gives the extruded forms a sense of depth.

## Screen-space depth and outlines

Screen-space ambient occlusion (SSAO) adds contact shadows and depth around surfaces. A per-building screen-space outline clarifies each silhouette and preserves the identity of individual buildings within dense blocks.

## Vertical gradient

Building sides use a vertical color gradient. The shift in tone communicates changes in height and creates additional separation between nearby forms.

## Selected building glow

The selected mass-timber building receives a screen-space glow, making the focused project immediately visible within the surrounding city.
