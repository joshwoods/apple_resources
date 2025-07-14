

- AVFoundation
- AVCaptureResolvedPhotoSettings
-  isStillImageStabilizationEnabled Deprecated

Instance Property

# isStillImageStabilizationEnabled

A Boolean value indicating whether this capture uses image stabilization.

iOS 10.0–13.0DeprecatediPadOS 10.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedtvOS 10.0–13.0Deprecated

``` source
var isStillImageStabilizationEnabled: Bool { get }
```

Deprecated

Use photoProcessingTimeRange instead.

## Discussion

This property corresponds to the AVCapturePhotoSettings property isAutoStillImageStabilizationEnabled.

When this value is true, the device automatically applies stabilization in low-light conditions to counteract hand shake. Automatic stabilization always includes digital image stabilization, and may also include optical lens stabilization, based on the current device.

If you specify automatic stabilization when requesting a capture, the device automatically chooses whether to use image stabilization based on the scene contents at the moment of capture. Therefore, you don’t know whether the system uses stabilization until right before the moment of capture. When the photo output calls your photoOutput(_:willBeginCaptureFor:) method (or other delegate methods that occur later in the capture process), you can use this property to determine whether stabilization is active.

## See Also

### Examining Photo Capture Settings

var isFlashEnabled: Bool

A Boolean value indicating whether the camera flash fires for this capture.

var isRedEyeReductionEnabled: Bool

A Boolean value indicating whether the camera automatically reduces red-eye when capturing photos.

var isVirtualDeviceFusionEnabled: Bool

A Boolean value that specifies whether the system automatically uses virtual device image fusion.

var isFastCapturePrioritizationEnabled: Bool

A Boolean value that indicates whether the system uses fast capture prioritization when capturing the photo.

var isContentAwareDistortionCorrectionEnabled: Bool

A Boolean value that indicates whether the system applies content-aware distortion correction when capturing the photo.

var isDualCameraFusionEnabled: Bool

A Boolean value indicating whether this capture combines image data from a dual camera.

Deprecated

