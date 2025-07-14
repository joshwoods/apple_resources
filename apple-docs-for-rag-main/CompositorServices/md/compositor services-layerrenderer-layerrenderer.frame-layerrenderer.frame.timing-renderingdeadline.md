

- Compositor Services
- LayerRenderer
- LayerRenderer.Frame
- LayerRenderer.Frame.Timing
-  renderingDeadline 

Instance Property

# renderingDeadline

The time at which you must finish all work for the specified frame.

visionOS 1.0+

``` source
var renderingDeadline: LayerRenderer.Clock.Instant { get }
```

## Discussion

This value reflects the time you need to finish your work and deliver the frame to Compositor Services. Finish all CPU tasks, commit your Metal command buffers, and call endSubmission() by the specified time. This time is before the actual presentation time of the frame, because it accounts for the Compositor Services overhead needed to render your frame and display it.

