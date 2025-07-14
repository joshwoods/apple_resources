

- AVFoundation
- AVCapturePhotoOutput
-  isContentAwareDistortionCorrectionSupported 

Instance Property

# isContentAwareDistortionCorrectionSupported

A Boolean value that indicates whether the session’s current configuration supports content-aware distortion correction.

iOS 14.1+iPadOS 14.1+Mac Catalyst 14.1+tvOS 17.0+

``` source
var isContentAwareDistortionCorrectionSupported: Bool { get }
```

## Discussion

Optical design and geometric distortion correction use a rectilinear model that preserves lines but not area, angles, or distance. The wider the field of view of a lens, the greater the areal distortion along the edges of images. Content-aware distortion correction intelligently adjusts its behavior to correct distortions based on the photo’s content. For example, the algorithm may not apply correction to faces in the center of a photo, but may apply it to faces near the photo’s edges.

Switching cameras or formats, or enabling depth data delivery, may result in a change to this property value. When the property changes from true to false, isContentAwareDistortionCorrectionEnabled also reverts to false.

This property is key-value observable.

## See Also

### Determining Available Settings

var isContentAwareDistortionCorrectionEnabled: Bool

A Boolean value that indicates whether the photo render pipeline can perform content-aware distortion correction.

var isLensStabilizationDuringBracketedCaptureSupported: Bool

A Boolean value indicating whether the capture output currently supports lens stabilization during bracketed image capture.

var maxBracketedCapturePhotoCount: Int

The maximum number of images that the photo capture output can support in a single bracketed capture.

var supportedFlashModes: [AVCaptureDevice.FlashMode]

A Swift array of flash settings this capture output currently supports.

var isAutoRedEyeReductionSupported: Bool

A Boolean value indicating whether the capture output supports automatic red-eye reduction.

