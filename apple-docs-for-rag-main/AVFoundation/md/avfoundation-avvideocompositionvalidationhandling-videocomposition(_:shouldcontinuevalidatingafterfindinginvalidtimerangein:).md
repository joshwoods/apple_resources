

- AVFoundation
- AVVideoCompositionValidationHandling
-  videoComposition(\_:shouldContinueValidatingAfterFindingInvalidTimeRangeIn:) 

Instance Method

# videoComposition(\_:shouldContinueValidatingAfterFindingInvalidTimeRangeIn:)

Reports a video composition instruction with a time range that is invalid.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+

``` source
optional func videoComposition(
    _ videoComposition: AVVideoComposition,
    shouldContinueValidatingAfterFindingInvalidTimeRangeIn videoCompositionInstruction: any AVVideoCompositionInstructionProtocol
) -> Bool
```

## Parameters 

`videoComposition`  

The video composition being validated.

`videoCompositionInstruction`  

The video composition instruction.

## Return Value

true if the video composition should continue validation in order to report additional problems that may exist, otherwise false.

## Discussion

A time range is considered invalid when it overlaps with the time range of a prior instruction, or that contains times earlier than the time range of a prior instruction

## See Also

### Configuring Validation Methods

func videoComposition(AVVideoComposition, shouldContinueValidatingAfterFindingInvalidValueForKey: String) -> Bool

Reports that a key that has an invalid value.

func videoComposition(AVVideoComposition, shouldContinueValidatingAfterFindingEmptyTimeRange: CMTimeRange) -> Bool

Reports a time range that has no corresponding video composition instruction.

func videoComposition(AVVideoComposition, shouldContinueValidatingAfterFindingInvalidTrackIDIn: any AVVideoCompositionInstructionProtocol, layerInstruction: AVVideoCompositionLayerInstruction, asset: AVAsset) -> Bool

Reports a video composition layer instruction that does not correspond to the track ID used for the composition’s animation or to a track of the asset.

