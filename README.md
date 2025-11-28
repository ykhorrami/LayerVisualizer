# Visualizer for LayerViews
Layer views define how your design will be visualized. 
This includes the color of each layer, the fill pattern, and whether the layer is visible or not. 
These settings are applied to the matplotlib plots, 3D views, cross-sections, and the settings can be exported to file for use in KLayout, too.
(Source: https://byucamacholab.github.io/Photonics-Bootcamp/pages/layer_stack.html)

## We have written code to change the following LayerViews:


https://github.com/ykhorrami/LayerVisualizer/blob/main/LayerView.py


----
## To be viewed using Python directly as follows:
#### (without .lyp format: https://github.com/ykhorrami/LayerVisualizer/blob/main/generic_tech.lyp)

:smiley:

![alt text](https://github.com/ykhorrami/LayerVisualizer/blob/main/1.png)

![alt text](https://github.com/ykhorrami/LayerVisualizer/blob/main/2.png)

# Note:

#### In integrated circuit and photonic design, layers are categorized based on their purpose and usage:

## 1. Main Layers
These are the actual fabrication layers used to create the physical structures on the chip:

  - Waveguide - Optical waveguides for light propagation

  - SLAB150 - Slab waveguides or partial etch regions

  - M1 - Metal 1 layer for electrical interconnects

  - VIA - Via connections between metal layers

  - TE/TM - Polarization-specific optical layers

  - DevRec - Device recognition/outline layers

  - PinRec - Pin recognition for electrical connections

  - Text - Text annotation layers

  - WG_PIN - Waveguide pin connections

## 2. XSECTION (Cross-Section) Layers
These are virtual layers used only for visualization and documentation of the chip's vertical cross-section structure. They represent the different material layers in the fabrication stack:

  - XS_BOX - Buried oxide layer

  - XS_SI - Silicon layer

  - XS_SI_SLAB - Silicon slab layer

  - XS_OX_SI - Oxide on silicon

  - XS_VIA - Via cross-section

  - XS_M1 - Metal 1 cross-section

  - XS_OXIDE_M1 - Oxide around metal 1

Key Differences:

| Aspect |	Main Layers |	XSECTION Layers|
| ------------- | ------------- | ------------- |
| `Purpose` |	Actual fabrication	| Visualization only|
| `Usage`	| Mask generation	| Documentation|
| `Physical`	| Real structures	| Virtual representation|
| `In GDS`	| Written to file	| Not written to masks|
