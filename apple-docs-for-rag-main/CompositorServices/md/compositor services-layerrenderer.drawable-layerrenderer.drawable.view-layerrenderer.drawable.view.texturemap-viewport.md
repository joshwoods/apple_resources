

- Compositor Services
- LayerRenderer
- 
  - LayerRenderer
- LayerRenderer.Drawable
- LayerRenderer.Drawable.View
- LayerRenderer.Drawable.View.TextureMap
-  viewport 

Instance Property

# viewport

The portion of the texture that the view uses to draw its content.

visionOS 1.0+

``` source
var viewport: MTLViewport { get }
```

## Discussion

This retrieves the size of the view and its location within the texture. If the layer dedicates a separate texture to each view, the texture bounds and view bounds match. However, if the layer uses a shared or layered texture, the view’s location or other slice index might differ.

## See Also

### Getting the view’s texture map

var textureMap: LayerRenderer.Drawable.View.TextureMap

The texture map for a view.

var textureIndex: Int

The index of the view’s textures in the drawable.

var sliceIndex: Int

The index of the view’s texture in an array-based texture type.

