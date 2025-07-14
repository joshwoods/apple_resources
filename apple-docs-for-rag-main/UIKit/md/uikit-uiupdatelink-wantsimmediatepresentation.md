

- UIKit
- UIUpdateLink
-  wantsImmediatePresentation 

Instance Property

# wantsImmediatePresentation

A Boolean value that determines whether the UI update link requests immediate frame presentation.

iOS 18.0+iPadOS 18.0+tvOS 18.0+visionOS 2.0+

``` source
@MainActor
var wantsImmediatePresentation: Bool { get set }
```

## Discussion

By default, the value of this property is false.

When the value of this property is true, the system requests immediate rendering of the display frame after the last CATransaction commit for the current UI update. Opting in to this behavior can help reduce latency between input and display because the rendered display frame presents one frame duration sooner. This behavior is primarily useful for pencil-drawing apps where low input-to-display latency is critical for an optimal user experience.

Important

If you opt in to this behavior, keep the complexity of the code you submit to the render server to a minimum. When an app requests immediate frame presentation, but doesn’t keep rendering complexity minimal, frames don’t submit for presentation in time. Dropped frames cause hitches and provide a suboptimal user experience. If you request immediate presentation, make sure to profile your app thoroughly. For more information, read Understanding user interface responsiveness.

## See Also

### Configuring preferences

var requiresContinuousUpdates: Bool

A Boolean value that determines whether the UI update link needs continuous UI updates.

var wantsLowLatencyEventDispatch: Bool

A Boolean value that determines whether the UI update link requests dispatch of low-latency eligible events.

var preferredFrameRateRange: CAFrameRateRange

The range of frame rates the UI update link prefers.

