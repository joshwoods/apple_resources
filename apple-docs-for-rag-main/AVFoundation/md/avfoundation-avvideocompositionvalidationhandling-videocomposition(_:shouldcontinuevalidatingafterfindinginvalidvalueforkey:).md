

- AVFoundation
- AVVideoCompositionValidationHandling
-  videoComposition(\_:shouldContinueValidatingAfterFindingInvalidValueForKey:) 

Instance Method

# videoComposition(\_:shouldContinueValidatingAfterFindingInvalidValueForKey:)

Reports that a key that has an invalid value.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+

``` source
optional func videoComposition(
    _ videoComposition: AVVideoComposition,
    shouldContinueValidatingAfterFindingInvalidValueForKey key: String
) -> Bool
```

## Parameters 

`videoComposition`  

The video composition being validated.

`key`  

The key being validated.

## Return Value

true if the video composition should continue validation in order to report additional problems that may exist, otherwise false.

## See Also

### Configuring Validation Methods

func videoComposition(AVVideoComposition, shouldContinueValidatingAfterFindingEmptyTimeRange: CMTimeRange) -> Bool

Reports a time range that has no corresponding video composition instruction.

func videoComposition(AVVideoComposition, shouldContinueValidatingAfterFindingInvalidTimeRangeIn: any AVVideoCompositionInstructionProtocol) -> Bool

Reports a video composition instruction with a time range that is invalid.

func videoComposition(AVVideoComposition, shouldContinueValidatingAfterFindingInvalidTrackIDIn: any AVVideoCompositionInstructionProtocol, layerInstruction: AVVideoCompositionLayerInstruction, asset: AVAsset) -> Bool

Reports a video composition layer instruction that does not correspond to the track ID used for the composition’s animation or to a track of the asset.

