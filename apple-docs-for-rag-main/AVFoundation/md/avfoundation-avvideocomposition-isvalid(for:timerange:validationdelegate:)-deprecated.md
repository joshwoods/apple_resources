

- AVFoundation
- AVVideoComposition
-  isValid(for:timeRange:validationDelegate:) Deprecated

Instance Method

# isValid(for:timeRange:validationDelegate:)

Indicates whether the time ranges of the composition’s instructions conform to validation requirements.

iOS 5.0–18.0DeprecatediPadOS 5.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.8–15.0DeprecatedtvOS 9.0–18.0Deprecated

``` source
func isValid(
    for asset: AVAsset?,
    timeRange: CMTimeRange,
    validationDelegate: (any AVVideoCompositionValidationHandling)?
) -> Bool
```

Deprecated

Use isValid(for:assetDuration:timeRange:validationDelegate:) instead.

## Parameters 

`asset`  

An asset object, if you require validating the time ranges of the instructions against the duration of the asset and the track IDs of the layer instructions against the asset’s tracks.

Pass `nil` to skip that validation.

`timeRange`  

A time range over which to validate instructions. The method validates only instructions with time ranges that overlap with this time range. To validate all instructions that you can use for playback or other processing, regardless of time range, pass `CMTimeRange(start: .zero, duration: .positiveInfinity)`.

`validationDelegate`  

An object that adopts the AVVideoCompositionValidationHandling protocol to receive detailed information about problematic sections of a video composition during processing.

Pass `nil` if you don’t require the details.

## Return Value

true if the time ranges of the composition’s instructions conform to validation requirements, otherwise false.

## Discussion

Apple discourages using this method in iOS 16, tvOS 16, and macOS 13 or later. Use determineValidity(for:timeRange:validationDelegate:completionHandler:) instead.

During validation, the video composition calls the validation delegate, if one exists, with a reference to any trouble spots in the video composition.

This method raises an exception if the delegate modifies the video composition’s instructions, or the array of layer instructions of any AVVideoCompositionInstruction object contained therein during validation.

## See Also

### Validating the Time Range

func isValid(for: [AVAssetTrack], assetDuration: CMTime, timeRange: CMTimeRange, validationDelegate: (any AVVideoCompositionValidationHandling)?) -> Bool

Indicates whether the time ranges of the composition’s instructions conform to validation requirements.

protocol AVVideoCompositionValidationHandling

Methods you can implement to indicate whether validation of a video composition should continue after specific errors are found.

func determineValidity(for: AVAsset?, timeRange: CMTimeRange, validationDelegate: (any AVVideoCompositionValidationHandling)?, completionHandler: (Bool, (any Error)?) -> Void)

Determines whether the time ranges of the composition’s instructions conform to validation requirements.

Deprecated

