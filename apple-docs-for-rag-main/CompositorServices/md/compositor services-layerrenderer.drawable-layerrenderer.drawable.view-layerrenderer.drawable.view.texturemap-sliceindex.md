

- Compositor Services
- LayerRenderer
- 
  - LayerRenderer
- LayerRenderer.Drawable
- LayerRenderer.Drawable.View
- LayerRenderer.Drawable.View.TextureMap
-  sliceIndex 

Instance Property

# sliceIndex

The index of the view’s texture in an array-based texture type.

visionOS 1.0+

``` source
var sliceIndex: Int { get }
```

## Discussion

Use the returned index to retrieve the view’s texture when the texture type is MTLTextureType.type2DArray. When configuring your render pass descriptor, specify the index in the slice property of the descriptor’s color and depth attachments.

If you don’t use array-based textures for drawing, fetch the index using textureIndex instead.

## See Also

### Getting the view’s texture map

var textureMap: LayerRenderer.Drawable.View.TextureMap

The texture map for a view.

var textureIndex: Int

The index of the view’s textures in the drawable.

var viewport: MTLViewport

The portion of the texture that the view uses to draw its content.

