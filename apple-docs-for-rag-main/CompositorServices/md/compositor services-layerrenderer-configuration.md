

- Compositor Services
- LayerRenderer
-  configuration 

Instance Property

# configuration

The configuration details for the specified layer.

visionOS 1.0+

``` source
var configuration: LayerRenderer.Configuration { get }
```

## Discussion

Use the information in this property to set up your rendering loop. The layer ignores any modifications you make to the specified configuration data. To properly configure the layer, specify those details in the initializer for your CompositorLayer type.

## See Also

### Configuring the layer renderer

struct Configuration

A type that stores the texture formats, layout information, and other details you use to configure your rendering loop code.

struct Capabilities

The color formats, depth formats, and features that you can use to configure your rendering engine.

