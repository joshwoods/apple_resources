

- Compositor Services
- LayerRenderer
- LayerRenderer.Drawable
-  views 

Instance Property

# views

An array of viewports that tell you how to draw to the drawable’s textures

visionOS 1.0+

``` source
var views: [LayerRenderer.Drawable.View] { get }
```

## Discussion

The drawable provides one view for each distinct image you need to render. For example, a stereoscopic display contains a separate view for each eye.

## See Also

### Getting the views

struct View

A type that provides information on how to render content into the frame’s textures.

