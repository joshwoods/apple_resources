

- Compositor Services
- TextureTopology
-  textureType 

Instance Property

# textureType

The texture type value that specifies how the underlying texture organizes its views.

visionOS 1.0+

``` source
var textureType: MTLTextureType { get }
```

## Discussion

A texture might store the content of one view or multiple views. For example, a single texture might store one or both views for the left and right eyes of a head-mounted display. The texture type indicates this content organization strategy.

## See Also

### Getting the layer’s texture topology

var arrayLength: UInt64

The number of items in the texture array.

