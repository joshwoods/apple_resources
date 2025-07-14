

- Compositor Services
- LayerRenderer
- LayerRenderer.Configuration
-  depthUsage 

Instance Property

# depthUsage

The texture usage value to apply to the layer’s depth textures.

visionOS 1.0+

``` source
var depthUsage: MTLTextureUsage { get set }
```

## Discussion

Metal optimizes texture-related operations based on the value in this property. The usage value can be a combination of options. For more information, see MTLTextureUsage.

## See Also

### Configuring the depth information

var depthFormat: MTLPixelFormat

The pixel format to use for the layer’s depth textures.

var defaultDepthRange: SIMD2&lt;Float>

The distances to the far and near clipping planes that define the bounds of your content.

