

- Compositor Services
- LayerRenderer
- LayerRenderer.Frame
-  predictTiming() 

Instance Method

# predictTiming()

Computes and returns the predicted timing information for the frame.

visionOS 1.0+

``` source
func predictTiming() -> LayerRenderer.Frame.Timing?
```

## Return Value

The predicted timing information for the specified frame, or `nil` if the layer is in the `Layer.State.paused` or `Layer.State.invalidated` state.

## Mentioned in 

Drawing fully immersive content using Metal

## Discussion

The returned timing information contains the frame-related deadlines to meet during the rendering process. For example, wait until the time in `optimalInputTime` to start the submission phase of your frame update. This function updates the frame-specific timing information with the latest data from Compositor Services before it returns it.

Don’t call this function after you call queryDrawable() for the specified frame. After you retrieve the frame’s LayerRenderer.Drawable type, get the timing information from the drawable’s frameTiming property instead.

## See Also

### Getting timing information

struct Timing

A type that stores information about a frame’s encoding, rendering, and presentation deadlines.

