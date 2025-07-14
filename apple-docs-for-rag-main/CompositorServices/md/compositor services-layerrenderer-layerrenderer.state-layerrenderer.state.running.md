

- Compositor Services
- LayerRenderer
- LayerRenderer.State
-  LayerRenderer.State.running 

Case

# LayerRenderer.State.running

A state that indicates the layer is visible and ready for you to draw your content.

visionOS 1.0+

``` source
case running
```

## Mentioned in 

Drawing fully immersive content using Metal

## Discussion

When the layer enters this state, start your rendering loop and begin drawing frames of content. Keep drawing frames of content until the layer transitions to another state.

## See Also

### Getting the states

case paused

A state that indicates the layer is paused and not currently drawing.

case invalidated

A state that indicates the layer no longer supports drawing operations.

