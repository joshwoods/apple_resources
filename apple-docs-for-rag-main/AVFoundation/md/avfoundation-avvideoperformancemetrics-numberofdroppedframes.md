

- AVFoundation
- AVVideoPerformanceMetrics
-  numberOfDroppedFrames 

Instance Property

# numberOfDroppedFrames

The total number of frames the system drops prior to decoding or from missing the display deadline.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+macOS 14.4+tvOS 17.4+visionOS 1.1+

``` source
var numberOfDroppedFrames: Int { get }
```

## See Also

### Inspecting metrics

var totalNumberOfFrames: Int

The total number of frames that display if no frames drop.

var numberOfCorruptedFrames: Int

The total number of corrupted frames.

var numberOfFramesDisplayedUsingOptimizedCompositing: Int

The total number of full screen frames rendered in a special power-efficient mode that didn’t require compositing with other UI elements.

var totalAccumulatedFrameDelay: TimeInterval

The accumulated amount of time between the prescribed presentation times of displayed video frames and their actual time of display.

