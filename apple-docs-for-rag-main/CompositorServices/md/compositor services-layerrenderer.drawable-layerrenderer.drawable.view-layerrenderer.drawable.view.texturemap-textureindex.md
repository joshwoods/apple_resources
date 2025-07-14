

- Compositor Services
- LayerRenderer
- 
  - LayerRenderer
- LayerRenderer.Drawable
- LayerRenderer.Drawable.View
- LayerRenderer.Drawable.View.TextureMap
-  textureIndex 

Instance Property

# textureIndex

The index of the view’s textures in the drawable.

visionOS 1.0+

``` source
var textureIndex: Int { get }
```

## Discussion

Compositor Services places the color and depth textures for this view at same index number in the drawable. Use the returned index to the colorTextures or depthTextures properties to retrieve the appropriate texture.

Compositor Services places the color and depth textures for this view at same index number in the drawable. In Swift, the index applies to the colorTexturesand depthTextures properties. In ObjectiveC, the index applies to the cp_drawable_get_color_texture and cp_drawable_get_depth_texture functions.

Note

If you draw with array-based textures, retrieve and apply the index from sliceIndex instead.

## See Also

### Getting the view’s texture map

var textureMap: LayerRenderer.Drawable.View.TextureMap

The texture map for a view.

var sliceIndex: Int

The index of the view’s texture in an array-based texture type.

var viewport: MTLViewport

The portion of the texture that the view uses to draw its content.

