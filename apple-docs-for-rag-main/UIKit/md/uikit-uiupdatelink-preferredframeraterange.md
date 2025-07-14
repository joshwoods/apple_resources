

- UIKit
- UIUpdateLink
-  preferredFrameRateRange 

Instance Property

# preferredFrameRateRange

The range of frame rates the UI update link prefers.

iOS 18.0+iPadOS 18.0+tvOS 18.0+visionOS 2.0+

``` source
@MainActor
var preferredFrameRateRange: CAFrameRateRange { get set }
```

## Discussion

By default, the value of this property is default, which doesn’t request any specific frame rate range.

## See Also

### Configuring preferences

var requiresContinuousUpdates: Bool

A Boolean value that determines whether the UI update link needs continuous UI updates.

var wantsLowLatencyEventDispatch: Bool

A Boolean value that determines whether the UI update link requests dispatch of low-latency eligible events.

var wantsImmediatePresentation: Bool

A Boolean value that determines whether the UI update link requests immediate frame presentation.

