

- Compositor Services
- LayerRenderer
- LayerRenderer.State
-  LayerRenderer.State.paused 

Case

# LayerRenderer.State.paused

A state that indicates the layer is paused and not currently drawing.

visionOS 1.0+

``` source
case paused
```

## Mentioned in 

Drawing fully immersive content using Metal

## Discussion

A layer starts in this state and later transitions to other states over time. Don’t run your render loop or do any drawing while in this state. Wait until the layer changes to one of the other states to take further action.

## See Also

### Getting the states

case running

A state that indicates the layer is visible and ready for you to draw your content.

case invalidated

A state that indicates the layer no longer supports drawing operations.

