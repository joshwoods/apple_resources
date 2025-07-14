

- AVFoundation
- AVCaptureStillImageOutput
-  isLensStabilizationDuringBracketedCaptureSupported Deprecated

Instance Property

# isLensStabilizationDuringBracketedCaptureSupported

A Boolean value that indicates whether the capture output supports lens stabilization across the duration of a bracketed capture.

iOS 9.0–10.0DeprecatediPadOS 9.0–10.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
var isLensStabilizationDuringBracketedCaptureSupported: Bool { get }
```

Deprecated

Use AVCapturePhotoOutput lensStabilizationDuringBracketedCaptureSupported instead.

## Discussion

You may set the isLensStabilizationDuringBracketedCaptureEnabled property only if this property’s value is true. This value may change as the session’s sessionPreset property or the input device’s activeFormat property changes.

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

var isLensStabilizationDuringBracketedCaptureEnabled: Bool

A Boolean value that specifies whether to stabilize the lens across the duration of a bracketed capture.

Deprecated

