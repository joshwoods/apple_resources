

- AVFoundation
- AVCapturePhotoSettings
-  flashMode 

Instance Property

# flashMode

A setting for whether to fire the flash when capturing photos.

iOS 10.0+iPadOS 10.0+Mac Catalyst 14.0+macOS 13.0+tvOS 17.0+

``` source
var flashMode: AVCaptureDevice.FlashMode { get set }
```

## Discussion

The default value for this setting is AVCaptureDevice.FlashMode.off.

Note

This setting supersedes the deprecated AVCaptureDevice flashMode property. When using the AVCapturePhotoOutput class, the capture device’s flash mode doesn’t apply—use this property on your photo settings object instead.

Assuming a static scene, using the AVCaptureDevice.FlashMode.auto setting is equivalent to testing the AVCapturePhotoOutput isFlashScene property (which indicates whether flash is recommended for the scene currently visible to the camera), and then setting the flashMode property of your photo settings output accordingly before requesting a capture. However, the visible scene can change between when you request a capture and when the camera hardware captures an image—the automatic setting ensures that the flash is enabled or disabled appropriately at the moment of capture. When the capture occurs, your AVCapturePhotoCaptureDelegate methods receive an AVCaptureResolvedPhotoSettings object whose isFlashEnabled property indicates which flash mode was used for that capture.

Note

When the device becomes very hot, the flash becomes temporarily unavailable until the device cools down (see the AVCaptureDevice isFlashAvailable property). While the flash is unavailable, a photo output’s supportedFlashModes property still reports the AVCaptureDevice.FlashMode.on and AVCaptureDevice.FlashMode.auto options as available, so you can still enable the flash in your photo settings even when the flash is temporarily unavailable.

When the photo output calls your AVCapturePhotoCaptureDelegate methods, check the isFlashEnabled property of the provided AVCaptureResolvedPhotoSettings to verify whether the flash is in use.

When specifying a flash mode, the following requirements apply:

- The specified mode must be present in the photo output’s supportedFlashModes array.

- You may not enable image stabilization if the flash mode is AVCaptureDevice.FlashMode.on. (Enabling the flash takes priority over the isAutoStillImageStabilizationEnabled setting).

The capture output validates these requirements when you call the capturePhoto(with:delegate:) method. If your settings don’t meet these requirements, that method raises an exception.

## See Also

### Configuring photo settings

var isAutoRedEyeReductionEnabled: Bool

A Boolean value that indicates whether to use auto red-eye reduction on flash captures.

var maxPhotoDimensions: CMVideoDimensions

The maximum resolution of the photo to capture.

var photoQualityPrioritization: AVCapturePhotoOutput.QualityPrioritization

A setting that indicates how to prioritize photo quality against speed of photo delivery.

var isCameraCalibrationDataDeliveryEnabled: Bool

A Boolean value that determines whether a dual photo capture also delivers camera calibration data.

var isAutoContentAwareDistortionCorrectionEnabled: Bool

A Boolean value that specifies whether the photo output, at its discretion, uses content-aware distortion correction on this photo request.

var isAutoVirtualDeviceFusionEnabled: Bool

A Boolean value that specifies whether to use automatic virtual-device image fusion.

var virtualDeviceConstituentPhotoDeliveryEnabledDevices: [AVCaptureDevice]

The constituent devices for which the virtual device should deliver photos.

var isDualCameraDualPhotoDeliveryEnabled: Bool

A Boolean value that determines whether a dual camera device delivers images from both cameras.

Deprecated

var isAutoDualCameraFusionEnabled: Bool

A Boolean value that specifies whether captures automatically combine data from a dual camera device.

Deprecated

var isAutoStillImageStabilizationEnabled: Bool

A Boolean value that specifies whether captures use automatic image stabilization.

Deprecated

var isHighResolutionPhotoEnabled: Bool

A Boolean value that specifies whether to capture still images at the highest resolution supported by the active device and format.

Deprecated

