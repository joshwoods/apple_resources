

- Compositor Services
- LayerRenderer
- LayerRenderer.Frame
-  queryDrawable() 

Instance Method

# queryDrawable()

Retrieves the frame’s drawable, which contains the textures and drawing environment for the frame.

visionOS 1.0+

``` source
func queryDrawable() -> LayerRenderer.Drawable?
```

## Return Value

The drawable type, or `nil` if the layer is in the LayerRenderer.State.paused or LayerRenderer.State.invalidated state.

## Discussion

Fetch the drawable when you’re ready to encode the drawing commands for the frame. The LayerRenderer.Drawable type contains the textures and other information you need to set up your render descriptor in Metal.

