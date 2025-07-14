

- Compositor Services
- LayerRenderer
- LayerRenderer.Configuration
-  depthFormat 

Instance Property

# depthFormat

The pixel format to use for the layer’s depth textures.

visionOS 1.0+

``` source
var depthFormat: MTLPixelFormat { get set }
```

## Discussion

Use this value to determine the pixel format for depth textures in a frame. At configuration time, set the value to specify which pixel format you want.

## See Also

### Configuring the depth information

var depthUsage: MTLTextureUsage

The texture usage value to apply to the layer’s depth textures.

var defaultDepthRange: SIMD2&lt;Float>

The distances to the far and near clipping planes that define the bounds of your content.

