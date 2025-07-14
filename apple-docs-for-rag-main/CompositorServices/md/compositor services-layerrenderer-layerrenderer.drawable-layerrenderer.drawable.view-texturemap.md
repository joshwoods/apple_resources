

- Compositor Services
- LayerRenderer
- LayerRenderer.Drawable
- LayerRenderer.Drawable.View
-  textureMap 

Instance Property

# textureMap

The texture map for a view.

visionOS 1.0+

``` source
var textureMap: LayerRenderer.Drawable.View.TextureMap { get }
```

## Discussion

Use the texture map to fetch additional information you need to draw your content. For example, use it to fetch the rectangle that defines the view’s content area.

## See Also

### Getting the view’s texture map

struct TextureMap

A type that provides details about the textures associated with a view.

