

- Compositor Services
- TextureTopology
-  arrayLength 

Instance Property

# arrayLength

The number of items in the texture array.

visionOS 1.0+

``` source
var arrayLength: UInt64 { get }
```

## Discussion

Array-based texture types such as MTLTextureType.type2DArray manage one or more images of the same size. The array length represents the number of separate images the texture manages. Other array types store only one image.

## See Also

### Getting the layer’s texture topology

var textureType: MTLTextureType

The texture type value that specifies how the underlying texture organizes its views.

