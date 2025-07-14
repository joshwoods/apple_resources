

- AVFoundation
- AVCapturePhotoOutput
-  isContentAwareDistortionCorrectionEnabled 

Instance Property

# isContentAwareDistortionCorrectionEnabled

A Boolean value that indicates whether the photo render pipeline can perform content-aware distortion correction.

iOS 14.1+iPadOS 14.1+Mac Catalyst 14.1+tvOS 17.0+

``` source
var isContentAwareDistortionCorrectionEnabled: Bool { get set }
```

## Discussion

You can set this value to true only if isContentAwareDistortionCorrectionSupported returns true.

Applying distortion correction to preserve natural-looking content may result in a small change in the field of view compared to what you see in AVCaptureVideoPreviewLayer. The amount lost or gained is content specific and varies from photo to photo.

Enabling this property requires a lengthy reconfiguration of the capture render pipeline, so set this property to true before calling startRunning() on the capture session.

## See Also

### Determining Available Settings

var isContentAwareDistortionCorrectionSupported: Bool

A Boolean value that indicates whether the session’s current configuration supports content-aware distortion correction.

var isLensStabilizationDuringBracketedCaptureSupported: Bool

A Boolean value indicating whether the capture output currently supports lens stabilization during bracketed image capture.

var maxBracketedCapturePhotoCount: Int

The maximum number of images that the photo capture output can support in a single bracketed capture.

var supportedFlashModes: [AVCaptureDevice.FlashMode]

A Swift array of flash settings this capture output currently supports.

var isAutoRedEyeReductionSupported: Bool

A Boolean value indicating whether the capture output supports automatic red-eye reduction.

