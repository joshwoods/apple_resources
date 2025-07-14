

- Compositor Services
- LayerRenderer
- LayerRenderer.State
-  LayerRenderer.State.invalidated 

Case

# LayerRenderer.State.invalidated

A state that indicates the layer no longer supports drawing operations.

visionOS 1.0+

``` source
case invalidated
```

## Mentioned in 

Drawing fully immersive content using Metal

## Discussion

A layer enters this state shortly before the system releases its resources. When the layer enters this state, exit your rendering loop and release any drawing-related structures.

## See Also

### Getting the states

case paused

A state that indicates the layer is paused and not currently drawing.

case running

A state that indicates the layer is visible and ready for you to draw your content.

