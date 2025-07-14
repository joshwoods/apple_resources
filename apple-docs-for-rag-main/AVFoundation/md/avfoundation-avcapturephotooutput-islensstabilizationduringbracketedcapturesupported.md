

- AVFoundation
- AVCapturePhotoOutput
-  isLensStabilizationDuringBracketedCaptureSupported 

Instance Property

# isLensStabilizationDuringBracketedCaptureSupported

A Boolean value indicating whether the capture output currently supports lens stabilization during bracketed image capture.

iOS 10.0+iPadOS 10.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
var isLensStabilizationDuringBracketedCaptureSupported: Bool { get }
```

## Discussion

To make use of optical image stabilization across the entire duration of a bracketed capture, set the isLensStabilizationEnabled property of your bracketed photo settings object.

Note

This property’s value can change if the sessionPreset property of the current capture session or the activeFormat property of the underlying capture device changes.

This property supports key-value observing.

## See Also

### Determining Available Settings

var isContentAwareDistortionCorrectionSupported: Bool

A Boolean value that indicates whether the session’s current configuration supports content-aware distortion correction.

var isContentAwareDistortionCorrectionEnabled: Bool

A Boolean value that indicates whether the photo render pipeline can perform content-aware distortion correction.

var maxBracketedCapturePhotoCount: Int

The maximum number of images that the photo capture output can support in a single bracketed capture.

var supportedFlashModes: [AVCaptureDevice.FlashMode]

A Swift array of flash settings this capture output currently supports.

var isAutoRedEyeReductionSupported: Bool

A Boolean value indicating whether the capture output supports automatic red-eye reduction.

