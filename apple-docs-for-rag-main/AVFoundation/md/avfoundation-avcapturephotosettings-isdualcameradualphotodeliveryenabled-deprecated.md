

- AVFoundation
- AVCapturePhotoSettings
-  isDualCameraDualPhotoDeliveryEnabled Deprecated

Instance Property

# isDualCameraDualPhotoDeliveryEnabled

A Boolean value that determines whether a dual camera device delivers images from both cameras.

iOS 11.0–13.0DeprecatediPadOS 11.0–13.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
var isDualCameraDualPhotoDeliveryEnabled: Bool { get set }
```

## Discussion

When this property is false (the default), and the photo output is configured with a capture device of the builtInDualCamera type, the photo output delivers a single main photo image for each capture. (The device determines how to produce that image from one or both cameras).

If you change this setting to true, your delegate’s photoOutput(_:didFinishProcessingPhoto:error:) method fires at least twice for each main image—once for the telephoto image and again for the wide-angle image. Setting this property to true when not using a dual-camera device raises an exception.

## See Also

### Configuring photo settings

var flashMode: AVCaptureDevice.FlashMode

A setting for whether to fire the flash when capturing photos.

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

var isAutoDualCameraFusionEnabled: Bool

A Boolean value that specifies whether captures automatically combine data from a dual camera device.

Deprecated

var isAutoStillImageStabilizationEnabled: Bool

A Boolean value that specifies whether captures use automatic image stabilization.

Deprecated

var isHighResolutionPhotoEnabled: Bool

A Boolean value that specifies whether to capture still images at the highest resolution supported by the active device and format.

Deprecated

