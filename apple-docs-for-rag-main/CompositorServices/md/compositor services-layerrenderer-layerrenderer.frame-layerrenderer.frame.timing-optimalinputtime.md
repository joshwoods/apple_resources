

- Compositor Services
- LayerRenderer
- LayerRenderer.Frame
- LayerRenderer.Frame.Timing
-  optimalInputTime 

Instance Property

# optimalInputTime

The optimal time to start the frame submission process.

visionOS 1.0+

``` source
var optimalInputTime: LayerRenderer.Clock.Instant { get }
```

## Discussion

The optimal input time is the time at which to call the startSubmission() function and begin encoding your Metal command buffers. Use the time before the input time to update your app’s data structures and prepare for rendering. Call wait(until:tolerance:) to suspend your app until the optimal time arrives. When it does, fetch the current device pose and finish rendering and the frame and commit your Metal command buffers.

