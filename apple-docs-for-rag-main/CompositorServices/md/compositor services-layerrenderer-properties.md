

- Compositor Services
- LayerRenderer
-  properties 

Instance Property

# properties

The configured properties of the layer renderer.

visionOS 1.0+

``` source
var properties: LayerRenderer.Properties { get }
```

## Discussion

The layer properties include details about the layer’s textures, such as their organization and the location of drawable views in those textures.

## See Also

### Getting the layer renderer properties

struct Properties

A type that describes the organization of the layer renderer’s textures and the relationships between those textures and the views you use for drawing.

