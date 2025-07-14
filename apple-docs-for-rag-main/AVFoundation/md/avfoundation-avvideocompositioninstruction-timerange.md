

- AVFoundation
- AVVideoCompositionInstruction
-  timeRange 

Instance Property

# timeRange

The time range to which the instruction applies.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
var timeRange: CMTimeRange { get }
```

## Discussion

If the time range is invalid, the video compositor will ignore it. See also the requirements of the timeRange property in the array of objects implementing the AVVideoCompositionInstructionProtocol protocol as described in the AVVideoComposition class’s instructions property.

## See Also

### Inspecting the Instruction

var backgroundColor: CGColor?

The background color of the composition.

var layerInstructions: [AVVideoCompositionLayerInstruction]

Instructions that specify how to layer and compose video frames from source tracks.

var enablePostProcessing: Bool

A Boolean value that indicates whether the instruction requires post processing.

