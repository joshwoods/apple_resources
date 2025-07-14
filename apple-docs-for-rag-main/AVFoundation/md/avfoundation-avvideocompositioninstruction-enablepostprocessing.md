

- AVFoundation
- AVVideoCompositionInstruction
-  enablePostProcessing 

Instance Property

# enablePostProcessing

A Boolean value that indicates whether the instruction requires post processing.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
var enablePostProcessing: Bool { get }
```

## Discussion

A value of false indicates that no post processing is required for the whole duration of the video composition instruction. The composition process is more efficient if the value is false.

The value is true by default.

## See Also

### Inspecting the Instruction

var backgroundColor: CGColor?

The background color of the composition.

var layerInstructions: [AVVideoCompositionLayerInstruction]

Instructions that specify how to layer and compose video frames from source tracks.

var timeRange: CMTimeRange

The time range to which the instruction applies.

