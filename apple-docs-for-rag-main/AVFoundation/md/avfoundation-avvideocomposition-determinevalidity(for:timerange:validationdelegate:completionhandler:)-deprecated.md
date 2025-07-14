

- AVFoundation
- AVVideoComposition
-  determineValidity(for:timeRange:validationDelegate:completionHandler:) Deprecated

Instance Method

# determineValidity(for:timeRange:validationDelegate:completionHandler:)

Determines whether the time ranges of the composition’s instructions conform to validation requirements.

iOS 16.0–18.0DeprecatediPadOS 16.0–18.0DeprecatedMac Catalyst 16.0–18.0DeprecatedmacOS 13.0–15.0DeprecatedtvOS 16.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
func determineValidity(
    for asset: AVAsset?,
    timeRange: CMTimeRange,
    validationDelegate: (any AVVideoCompositionValidationHandling)?,
    completionHandler: @escaping (Bool, (any Error)?) -> Void
)
```

``` source
func isValid(
    for asset: AVAsset?,
    timeRange: CMTimeRange,
    validationDelegate: (any AVVideoCompositionValidationHandling)?
) async throws -> Bool
```

Deprecated

Use isValid(for:assetDuration:timeRange:validationDelegate:) instead.

## Parameters 

`asset`  

An asset object, if you require validating the time ranges of the instructions against the duration of the asset and the track IDs of the layer instructions against the asset’s tracks. Pass `nil` to skip that validation.

`timeRange`  

A time range over which to validate instructions. The method validates only instructions with time ranges that overlap with this time range. To validate all instructions that you can use for playback or other processing, regardless of time range, pass `CMTimeRange(start: .zero, duration: .positiveInfinity)`.

`validationDelegate`  

An object that adopts the AVVideoCompositionValidationHandling protocol to receive detailed information about problematic sections of a video composition during processing. Pass `nil` if you don’t require the details.

`completionHandler`  

A block the system calls when it determines whether the video composition is valid.

## Discussion

During validation, the video composition calls the validation delegate, if one exists, with a reference to any trouble spots in the video composition.

This method raises an exception if the delegate modifies the video composition’s instructions, or the array of layer instructions of any AVVideoCompositionInstruction object contained therein during validation.

## See Also

### Validating the Time Range

func isValid(for: [AVAssetTrack], assetDuration: CMTime, timeRange: CMTimeRange, validationDelegate: (any AVVideoCompositionValidationHandling)?) -> Bool

Indicates whether the time ranges of the composition’s instructions conform to validation requirements.

protocol AVVideoCompositionValidationHandling

Methods you can implement to indicate whether validation of a video composition should continue after specific errors are found.

func isValid(for: AVAsset?, timeRange: CMTimeRange, validationDelegate: (any AVVideoCompositionValidationHandling)?) -> Bool

Indicates whether the time ranges of the composition’s instructions conform to validation requirements.

Deprecated

