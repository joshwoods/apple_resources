

- AVFoundation
- AVCapturePhotoSettings
-  isHighResolutionPhotoEnabled Deprecated

Instance Property

# isHighResolutionPhotoEnabled

A Boolean value that specifies whether to capture still images at the highest resolution supported by the active device and format.

iOS 10.0–16.0DeprecatediPadOS 10.0–16.0DeprecatedMac Catalyst 14.0–16.0DeprecatedmacOS 10.15–13.0Deprecated

``` source
var isHighResolutionPhotoEnabled: Bool { get set }
```

Deprecated

Use maxPhotoDimensions instead.

## Discussion

When this setting is false (the default), a photo capture output delivers images with the dimensions specified by the formatDescription property of the source AVCaptureDevice object’s active capture format. However, some devices and capture formats allow for still image capture at resolutions higher than their video capture (and streaming photo preview) resolution. To capture the highest possible resolution for still photos (described by the capture format’s highResolutionStillImageDimensions property), change this setting to true.

If any output connected to your capture session enables video stabilization (see the AVCaptureConnection preferredVideoStabilizationMode property), captured images may be around 10% smaller than the maximum still image dimensions. (This size change is an effect of video stabilization, which works by cropping and rotating to find the stable region in a moving image). Examine the AVCaptureResolvedPhotoSettings object provided to your photo capture delegate to find the actual dimensions of each captured photo.

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

var isAutoDualCameraFusionEnabled: Bool

A Boolean value that specifies whether captures automatically combine data from a dual camera device.

Deprecated

var isAutoStillImageStabilizationEnabled: Bool

A Boolean value that specifies whether captures use automatic image stabilization.

Deprecated

