

- AVFoundation
- AVCapturePhotoOutput
-  supportedFlashModes 

Instance Property

# supportedFlashModes

A Swift array of flash settings this capture output currently supports.

iOS 10.0+iPadOS 10.0+Mac Catalyst 14.0+macOS 11.0+tvOS 17.0+

``` source
@nonobjc
var supportedFlashModes: [AVCaptureDevice.FlashMode] { get }
```

## Discussion

To set the flash mode for a capture, set the flashMode property of your photo settings object to one of the AVCaptureDevice.FlashMode values listed in this array.

This property supports Key-Value Observing.

## See Also

### Determining Available Settings

var isContentAwareDistortionCorrectionSupported: Bool

A Boolean value that indicates whether the session’s current configuration supports content-aware distortion correction.

var isContentAwareDistortionCorrectionEnabled: Bool

A Boolean value that indicates whether the photo render pipeline can perform content-aware distortion correction.

var isLensStabilizationDuringBracketedCaptureSupported: Bool

A Boolean value indicating whether the capture output currently supports lens stabilization during bracketed image capture.

var maxBracketedCapturePhotoCount: Int

The maximum number of images that the photo capture output can support in a single bracketed capture.

var isAutoRedEyeReductionSupported: Bool

A Boolean value indicating whether the capture output supports automatic red-eye reduction.

