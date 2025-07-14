

- Compositor Services
- LayerRenderer
- LayerRenderer.Properties
-  init(configuration:) 

Initializer

# init(configuration:)

Creates a set of properties using the specified configuration values.

visionOS 1.0+

``` source
init(configuration: LayerRenderer.Configuration) throws
```

## Parameters 

`configuration`  

The options you use to configure your Metal rendering engine. Specify the same options you use during drawing.

## Discussion

Prior to receiving the layer you use for drawing, you can create a LayerRenderer.Properties structure and use it to start the configuration of your Metal code.

