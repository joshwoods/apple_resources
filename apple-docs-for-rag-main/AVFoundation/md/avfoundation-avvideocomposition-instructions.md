

- AVFoundation
- AVVideoComposition
-  instructions 

Instance Property

# instructions

The video composition instructions.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
var instructions: [any AVVideoCompositionInstructionProtocol] { get }
```

## Discussion

The array contains instances of AVVideoCompositionInstruction. For the first instruction in the array, `timeRange.start` must be less than or equal to the earliest time for which playback or other processing will be attempted (typically `kCMTimeZero`). For subsequent instructions, `timeRange.start` must be equal to the prior instruction’s end time. The end time of the last instruction must be greater than or equal to the latest time for which playback or other processing will be attempted (typically be the duration of the asset with which the instance of `AVVideoComposition` is associated).

## See Also

### Reading Instructions

protocol AVVideoCompositionInstructionProtocol

A protocol that defines the interface for a video composition instruction.

