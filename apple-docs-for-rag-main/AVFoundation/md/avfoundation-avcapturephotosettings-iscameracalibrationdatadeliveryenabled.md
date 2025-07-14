

- AVFoundation
- AVCapturePhotoSettings
-  isCameraCalibrationDataDeliveryEnabled 

Instance Property

# isCameraCalibrationDataDeliveryEnabled

A Boolean value that determines whether a dual photo capture also delivers camera calibration data.

iOS 11.0+iPadOS 11.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
var isCameraCalibrationDataDeliveryEnabled: Bool { get set }
```

## Discussion

When this setting is false (the default), and the isDualCameraDualPhotoDeliveryEnabled setting is true, dual photo capture doesn’t deliver additional data.

If you change this setting to true, the AVCapturePhoto results from a dual photo capture include AVCameraCalibrationData objects that describe the imaging parameters for each camera. This data can be useful for performing computer vision tasks on the resulting images.

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

