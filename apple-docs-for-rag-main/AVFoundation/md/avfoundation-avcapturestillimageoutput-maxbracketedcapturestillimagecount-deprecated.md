

- AVFoundation
- AVCaptureStillImageOutput
-  maxBracketedCaptureStillImageCount Deprecated

Instance Property

# maxBracketedCaptureStillImageCount

Specifies the maximum number of still images that may be taken in a single bracket.

iOS 8.0–10.0DeprecatediPadOS 8.0–10.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
var maxBracketedCaptureStillImageCount: Int { get }
```

Deprecated

Use AVCapturePhotoOutput maxBracketedCapturePhotoCount instead.

## Discussion

AVCaptureStillImageOutput can only satisfy a limited number of image requests in a single bracket without exhausting system resources.

The maximum number of still images that may be taken in a single bracket depends on the size of the images being captured, and consequently may vary with AVCaptureSession -sessionPreset and AVCaptureDevice -activeFormat values.

## See Also

### Related Documentation

func captureStillImageAsynchronously(from: AVCaptureConnection, completionHandler: (CMSampleBuffer?, (any Error)?) -> Void)

Initiates a still image capture and returns immediately.

Deprecated

### Still Image Bracketed Capture

func captureStillImageBracketAsynchronously(from: AVCaptureConnection, withSettingsArray: [AVCaptureBracketedStillImageSettings], completionHandler: (CMSampleBuffer?, AVCaptureBracketedStillImageSettings?, (any Error)?) -> Void)

Captures a still image bracket.

Deprecated

func prepareToCaptureStillImageBracket(from: AVCaptureConnection, withSettingsArray: [AVCaptureBracketedStillImageSettings], completionHandler: (Bool, (any Error)?) -> Void)

Allows the receiver to prepare resources in advance of capturing a still image bracket.

Deprecated

var isLensStabilizationDuringBracketedCaptureSupported: Bool

A Boolean value that indicates whether the capture output supports lens stabilization across the duration of a bracketed capture.

Deprecated

var isLensStabilizationDuringBracketedCaptureEnabled: Bool

A Boolean value that specifies whether to stabilize the lens across the duration of a bracketed capture.

Deprecated

