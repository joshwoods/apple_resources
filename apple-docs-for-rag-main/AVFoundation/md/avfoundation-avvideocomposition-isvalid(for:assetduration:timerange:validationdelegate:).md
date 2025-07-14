

- AVFoundation
- AVVideoComposition
-  isValid(for:assetDuration:timeRange:validationDelegate:) 

Instance Method

# isValid(for:assetDuration:timeRange:validationDelegate:)

Indicates whether the time ranges of the composition’s instructions conform to validation requirements.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
func isValid(
    for tracks: [AVAssetTrack],
    assetDuration duration: CMTime,
    timeRange: CMTimeRange,
    validationDelegate: (any AVVideoCompositionValidationHandling)?
) -> Bool
```

## Parameters 

`tracks`  

Pass a reference to an asset’s tracks if you wish to validate the track IDs of the layer instructions against the asset’s tracks. Pass `nil` to skip that validation. This method throws an exception if the tracks aren’t all from the same asset.

`duration`  

Pass the asset duration to validate the time ranges of the instructions. Pass invalid to skip that validation.

`timeRange`  

The composition only validates those instructions with time ranges that overlap with the specified time range. To validate all instructions that the composition may use for playback or other processing, regardless of time range, pass `CMTimeRange(start: .zero, end: .positiveInfinity)`.

`validationDelegate`  

A delegate that handles validation requests. May be `nil`.

## Return Value

true if the validation succeeds; otherwise; false.

## See Also

### Validating the Time Range

protocol AVVideoCompositionValidationHandling

Methods you can implement to indicate whether validation of a video composition should continue after specific errors are found.

func determineValidity(for: AVAsset?, timeRange: CMTimeRange, validationDelegate: (any AVVideoCompositionValidationHandling)?, completionHandler: (Bool, (any Error)?) -> Void)

Determines whether the time ranges of the composition’s instructions conform to validation requirements.

Deprecated

func isValid(for: AVAsset?, timeRange: CMTimeRange, validationDelegate: (any AVVideoCompositionValidationHandling)?) -> Bool

Indicates whether the time ranges of the composition’s instructions conform to validation requirements.

Deprecated

