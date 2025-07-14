

- AVFoundation
- AVCapturePhotoSettings
-  isAutoDualCameraFusionEnabled Deprecated

Instance Property

# isAutoDualCameraFusionEnabled

A Boolean value that specifies whether captures automatically combine data from a dual camera device.

iOS 10.2–13.0DeprecatediPadOS 10.2–13.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
var isAutoDualCameraFusionEnabled: Bool { get set }
```

## Discussion

The default setting is true, unless you are capturing a RAW photo. (By definition, RAW photos are unprocessed, and image fusion involves processing the captured image).

When you enable this setting, a dual-camera device automatically combines samples from both cameras to produce a higher quality image. This property applies only when using the builtInDualCamera device type on supported devices.

Tip

Image processing, including dual camera fusion, increases capture time. To capture photos at the highest possible speed (like in the built-in Camera app’s burst mode), set the isAutoDualCameraFusionEnabled and isAutoStillImageStabilizationEnabled properties to false and the flashMode property to AVCaptureDevice.FlashMode.off.

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

var isDualCameraDualPhotoDeliveryEnabled: Bool

A Boolean value that determines whether a dual camera device delivers images from both cameras.

Deprecated

var isAutoStillImageStabilizationEnabled: Bool

A Boolean value that specifies whether captures use automatic image stabilization.

Deprecated

var isHighResolutionPhotoEnabled: Bool

A Boolean value that specifies whether to capture still images at the highest resolution supported by the active device and format.

Deprecated

