

- Compositor Services
- LayerRenderer
- LayerRenderer.Drawable
-  depthTextures 

Instance Property

# depthTextures

An array of depth textures to use to render the current frame.

visionOS 1.0+

``` source
var depthTextures: [any MTLTexture] { get }
```

## Discussion

The layer’s texture topology determines the total number of textures in the array, and the layout and content for each texture. Use the drawable’s views to map your content into specific portions of the textures.

## See Also

### Getting the render textures

var colorTextures: [any MTLTexture]

An array of color textures to use to render the current frame.

