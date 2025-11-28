# Visualizer for LayerViews
Layer views define how your design will be visualized. 
This includes the color of each layer, the fill pattern, and whether the layer is visible or not. 
These settings are applied to the matplotlib plots, 3D views, cross-sections, and the settings can be exported to file for use in KLayout, too.
(Source: https://byucamacholab.github.io/Photonics-Bootcamp/pages/layer_stack.html)

## We write a code to change the following LayerViews:


LayerViews:

  Waveguide:
  
    layer: [1, 0]
    
    hatch_pattern: dotted
    
    width: 1
    
    color: "#ff9d9d"
    
  SLAB150:
  
    layer: [2, 0]
    
    layer_in_name: true
    
    hatch_pattern: coarsely dotted
    
    transparent: true
    
    width: 1
    
    color: "cyan"
    
  M1:
  
    layer: [41, 0]
    
    layer_in_name: true
    
    hatch_pattern: dotted
    
    width: 1
    
    color: "#01ff6b"
    
    brightness: -16
    
  VIA:
  
    layer: [40, 0]
    
    layer_in_name: true
    
    hatch_pattern: hollow
    
    width: 1
    
    color: "#cc4c00"
    
  LABEL_OPTICAL_IO:
  
    layer: [201, 0]
    
    layer_in_name: true
    
    hatch_pattern: hollow
    
    width: 1
    
    color: "blue"
    
  LABEL_SETTINGS:
  
    layer: [202, 0]
    
    layer_in_name: true
    
    hatch_pattern: hollow
    
    visible: false
    
    width: 1
    
    color: "magenta"
    
  TE:
  
    layer: [203, 0]
    
    layer_in_name: true
    
    transparent: true
    
    width: 1
    
    color: "blue"
    
  TM:
  
    layer: [204, 0]
    
    layer_in_name: true
    
    width: 1
    
    color: "red"
    
  LABEL_INSTANCES:
  
    layer: [206, 0]
    
    layer_in_name: true
    
    hatch_pattern: lightly left-hatched
    
    color: "blue"
    
  DevRec:
  
    layer: [68, 0]
    
    hatch_pattern: hollow
    
    visible: false
    
    transparent: true
    
    width: 1
    
    color: "#004080"
    
  PinRec:
  
    layer: [1, 10]
    
    hatch_pattern: hollow
    
    color: "#404040"
    
  Text:
  
    layer: [66, 0]
    
    hatch_pattern: hollow
    
    width: 1

    color: "blue"
    
  XSECTION:
  
    group_members:
    
      XS_BOX:
      
        layer: [300, 0]
        
        layer_in_name: true
        
        width: 1
        
        color: "#f3ff80"
        
        hatch_pattern: solid
        
      XS_SI:
      
        layer: [301, 0]
        
        layer_in_name: true
        
        width: 1
        
        color: "black"
        
        hatch_pattern: solid
        
      XS_SI_SLAB:
      
        layer: [313, 0]
        
        layer_in_name: true
        
        width: 1
        
        color: "#80a8ff"
        
        hatch_pattern: solid
        
      XS_OVERLAY:
      
        layer: [311, 0]
        
        layer_in_name: true
        
        width: 1
        
        color: "blue"
        
        hatch_pattern: solid
        
      XS_OX_SI:
      
        layer: [302, 0]
        
        layer_in_name: true
        
        width: 1
        
        color: "#f3ff80"
        
        hatch_pattern: solid
        
      XS_VIA:
      
        layer: [303, 0]
        
        layer_in_name: true
        
        width: 1
        
        color: "grey"
        
        hatch_pattern: solid
        
      XS_M1:
      
        layer: [304, 0]
        
        layer_in_name: true
        
        width: 1
        
        color: "green"
        
        hatch_pattern: solid
        
      XS_OXIDE_M1:
      
        layer: [305, 0]
        
        layer_in_name: true
        
        width: 1
        
        color: "#f3ff80"
        
        hatch_pattern: solid
        
      XS_VIA:
      
        layer: [308, 0]
        
        layer_in_name: true
        
        width: 1
        
        color: "grey"
        
        hatch_pattern: solid
        
  SHOW_PORTS:
  
    layer: [1, 12]
    
    layer_in_name: true
    
    hatch_pattern: lightly left-hatched
    
    color: "#ff80a8"
    
  WG_PIN:
  
    layer: [1, 10]
    
    layer_in_name: true
    
    hatch_pattern: lightly left-hatched
    
    color: "#ff80a8"


----
## Can be viewed using Python directly (without .lyp format: https://github.com/ykhorrami/LayerVisualizer/blob/main/generic_tech.lyp) as follows:
