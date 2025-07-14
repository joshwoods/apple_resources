

- AVFoundation
- AVVideoCompositionValidationHandling
-  videoComposition(\_:shouldContinueValidatingAfterFindingInvalidTrackIDIn:layerInstruction:asset:) 

Instance Method

# videoComposition(\_:shouldContinueValidatingAfterFindingInvalidTrackIDIn:layerInstruction:asset:)

Reports a video composition layer instruction that does not correspond to the track ID used for the composition’s animation or to a track of the asset.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+

``` source
optional func videoComposition(
    _ videoComposition: AVVideoComposition,
    shouldContinueValidatingAfterFindingInvalidTrackIDIn videoCompositionInstruction: any AVVideoCompositionInstructionProtocol,
    layerInstruction: AVVideoCompositionLayerInstruction,
    asset: AVAsset
) -> Bool
```

## Parameters 

`videoComposition`  

The video composition being validated.

`videoCompositionInstruction`  

The video composition instruction.

`layerInstruction`  

The layer instruction.

`asset`  

The underlying asset.

## Return Value

true if the video composition should continue validation in order to report additional problems that may exist, otherwise false.

## Discussion

The asset track is specified in the isValid(for:timeRange:validationDelegate:) method.

## See Also

### Configuring Validation Methods

func videoComposition(AVVideoComposition, shouldContinueValidatingAfterFindingInvalidValueForKey: String) -> Bool

Reports that a key that has an invalid value.

func videoComposition(AVVideoComposition, shouldContinueValidatingAfterFindingEmptyTimeRange: CMTimeRange) -> Bool

Reports a time range that has no corresponding video composition instruction.

func videoComposition(AVVideoComposition, shouldContinueValidatingAfterFindingInvalidTimeRangeIn: any AVVideoCompositionInstructionProtocol) -> Bool

Reports a video composition instruction with a time range that is invalid.

