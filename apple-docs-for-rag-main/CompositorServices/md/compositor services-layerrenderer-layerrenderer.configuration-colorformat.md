

- Compositor Services
- LayerRenderer
- LayerRenderer.Configuration
-  colorFormat 

Instance Property

# colorFormat

The pixel format to use for color textures.

visionOS 1.0+

``` source
var colorFormat: MTLPixelFormat { get set }
```

## Discussion

Use this value to determine the pixel format for color textures in a frame. At configuration time, set the value to specify which pixel format you want.

Note

Apple Vision Pro uses the P3 color space for pixel color values.

## See Also

### Configuring the color textures

var colorUsage: MTLTextureUsage

The texture usage value to apply to the layer’s color textures.

