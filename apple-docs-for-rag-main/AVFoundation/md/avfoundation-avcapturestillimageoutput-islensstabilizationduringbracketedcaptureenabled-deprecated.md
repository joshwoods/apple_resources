

- AVFoundation
- AVCaptureStillImageOutput
-  isLensStabilizationDuringBracketedCaptureEnabled Deprecated

Instance Property

# isLensStabilizationDuringBracketedCaptureEnabled

A Boolean value that specifies whether to stabilize the lens across the duration of a bracketed capture.

iOS 9.0–10.0DeprecatediPadOS 9.0–10.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
var isLensStabilizationDuringBracketedCaptureEnabled: Bool { get set }
```

Deprecated

Use AVCapturePhotoOutput with AVCapturePhotoBracketSettings instead.

## Discussion

Applying lens stabilization to bracketed capture attempts to keep the lens steady for the entire duration of the bracket, resulting in more consistent images across the bracket. When lens stabilization is enabled, bracketed still image captures incur additional latency. Lens stabilization is more effective with longer-exposure captures, and offers limited or no benefit for exposure durations shorter than 1/30 of a second. It is possible that during the bracket, the lens stabilization module may run out of correction range and therefore will not be active for every frame in the bracket. Each emitted sample buffer from the bracket has an attachment of `kCMSampleBufferAttachmentKey_StillImageLensStabilizationInfo` indicating additional information about stabilization applied to the buffer.

This property’s default value is false. You may set this property’s value to true only if the isLensStabilizationDuringBracketedCaptureSupported value is true. Otherwise, setting this property raises an exception (invalidArgumentException). If the isLensStabilizationDuringBracketedCaptureSupported property’s value changes to false, this property’s value also becomes false.

This property supports key-value observing.

## See Also

### Still Image Bracketed Capture

func captureStillImageBracketAsynchronously(from: AVCaptureConnection, withSettingsArray: [AVCaptureBracketedStillImageSettings], completionHandler: (CMSampleBuffer?, AVCaptureBracketedStillImageSettings?, (any Error)?) -> Void)

Captures a still image bracket.

Deprecated

var maxBracketedCaptureStillImageCount: Int

Specifies the maximum number of still images that may be taken in a single bracket.

Deprecated

func prepareToCaptureStillImageBracket(from: AVCaptureConnection, withSettingsArray: [AVCaptureBracketedStillImageSettings], completionHandler: (Bool, (any Error)?) -> Void)

Allows the receiver to prepare resources in advance of capturing a still image bracket.

Deprecated

var isLensStabilizationDuringBracketedCaptureSupported: Bool

A Boolean value that indicates whether the capture output supports lens stabilization across the duration of a bracketed capture.

Deprecated

