

- AVFoundation
- AVMutableVideoCompositionInstruction
-  timeRange 

Instance Property

# timeRange

The time range to which the instruction applies.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
var timeRange: CMTimeRange { get set }
```

## Discussion

If the time range is invalid, the video compositor ignores it.

## See Also

### Configuring the Instructions

var backgroundColor: CGColor?

The background color of the composition.

var layerInstructions: [AVVideoCompositionLayerInstruction]

Instructions that specify how to layer and compose video frames from source tracks.

var enablePostProcessing: Bool

A Boolean value that indicates whether the instruction requires post processing.

