

- Compositor Services
- LayerRenderer
- LayerRenderer.Drawable
-  frameTiming 

Instance Property

# frameTiming

The timing information for the drawable’s frame.

visionOS 1.0+

``` source
var frameTiming: LayerRenderer.Frame.Timing { get }
```

## Mentioned in 

Drawing fully immersive content using Metal

## Discussion

This retrieves a frame’s timing information from a drawable instance that represents that frame. For Swift, it’s an alternative to calling a frame’s predictTiming() method. For ObjectiveC, it’s an alternative to calling the cp_frame_predict_timing function.

In ObjectiveC, you can determine when to start updating your data structures by passing a cp_frame_timing_t instance to the cp_frame_timing_get_optimal_input_time function.

## See Also

### Synchronizing the drawing operation

var presentationFrameIndex: CompositorFrameIndex

The sequential index of a drawable’s frame.

