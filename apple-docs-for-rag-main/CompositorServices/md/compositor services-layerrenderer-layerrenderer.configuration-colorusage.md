

- Compositor Services
- LayerRenderer
- LayerRenderer.Configuration
-  colorUsage 

Instance Property

# colorUsage

The texture usage value to apply to the layer’s color textures.

visionOS 1.0+

``` source
var colorUsage: MTLTextureUsage { get set }
```

## Discussion

Metal optimizes texture-related operations based on the value in this property. The usage value can be a combination of options. For more information, see MTLTextureUsage.

## See Also

### Configuring the color textures

var colorFormat: MTLPixelFormat

The pixel format to use for color textures.

