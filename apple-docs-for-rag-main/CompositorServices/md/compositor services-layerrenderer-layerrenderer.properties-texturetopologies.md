

- Compositor Services
- LayerRenderer
- LayerRenderer.Properties
-  textureTopologies 

Instance Property

# textureTopologies

The texture topologies available for the layer.

visionOS 1.0+

``` source
var textureTopologies: [TextureTopology] { get }
```

## Discussion

Use the topology information to allocate the resources you need to manage your Metal data structures.

## See Also

### Getting the layer’s texture topology

struct TextureTopology

A type that specifies the organization of one of the drawable’s textures.

