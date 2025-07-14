

- AVFoundation
- AVCaptureResolvedPhotoSettings
-  isDualCameraFusionEnabled Deprecated

Instance Property

# isDualCameraFusionEnabled

A Boolean value indicating whether this capture combines image data from a dual camera.

iOS 10.2–13.0DeprecatediPadOS 10.2–13.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
var isDualCameraFusionEnabled: Bool { get }
```

Deprecated

Use isVirtualDeviceFusionEnabled instead.

## Discussion

This property corresponds to the AVCapturePhotoSettings property isAutoDualCameraFusionEnabled.

When this value is true, a dual-camera device automatically combines samples from both cameras to produce a higher quality image. This property applies only when using the builtInDualCamera device type on supported devices.

If you specify automatic image fusion when requesting a capture, the device automatically chooses whether to use image fusion based on the scene conditions at the moment of capture. Therefore, you don’t know whether the system uses image fusion until right before the moment of capture. When the photo output calls your photoOutput(_:willBeginCaptureFor:) method (or other delegate methods that occur later in the capture process), you can use this property to determine whether image fusion is active.

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

var isStillImageStabilizationEnabled: Bool

A Boolean value indicating whether this capture uses image stabilization.

Deprecated

