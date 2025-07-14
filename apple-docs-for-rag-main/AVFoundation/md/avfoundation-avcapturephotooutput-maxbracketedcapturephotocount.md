

- AVFoundation
- AVCapturePhotoOutput
-  maxBracketedCapturePhotoCount 

Instance Property

# maxBracketedCapturePhotoCount

The maximum number of images that the photo capture output can support in a single bracketed capture.

iOS 10.0+iPadOS 10.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
var maxBracketedCapturePhotoCount: Int { get }
```

## Discussion

To perform a bracketed capture of multiple images with varied capture settings, create a AVCapturePhotoBracketSettings instance containing the combination of settings and bracketed variations you want. The maximum number of photos per capture depends on the size and format of images to be captured.

Note

This property’s value can change if the sessionPreset property of the current capture session or the activeFormat property of the underlying capture device changes.

Not all devices and capture formats support bracketed capture. If the current device or active format does not support bracketed capture, this property’s value is zero.

This property supports key-value observing.

## See Also

### Determining Available Settings

var isContentAwareDistortionCorrectionSupported: Bool

A Boolean value that indicates whether the session’s current configuration supports content-aware distortion correction.

var isContentAwareDistortionCorrectionEnabled: Bool

A Boolean value that indicates whether the photo render pipeline can perform content-aware distortion correction.

var isLensStabilizationDuringBracketedCaptureSupported: Bool

A Boolean value indicating whether the capture output currently supports lens stabilization during bracketed image capture.

var supportedFlashModes: [AVCaptureDevice.FlashMode]

A Swift array of flash settings this capture output currently supports.

var isAutoRedEyeReductionSupported: Bool

A Boolean value indicating whether the capture output supports automatic red-eye reduction.

