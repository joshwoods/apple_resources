

- AVFoundation
- AVCapturePhotoSettings
-  isAutoVirtualDeviceFusionEnabled 

Instance Property

# isAutoVirtualDeviceFusionEnabled

A Boolean value that specifies whether to use automatic virtual-device image fusion.

iOS 13.0+iPadOS 13.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
var isAutoVirtualDeviceFusionEnabled: Bool { get set }
```

## Discussion

When isAutoVirtualDeviceFusionEnabled and isVirtualDeviceFusionSupported are true, the framework may fuse constituent camera images of a virtual device to improve still image quality, depending on the current zoom factor, light levels, and focus position. You can determine whether virtual device fusion is enabled for a particular capture request by inspecting the isVirtualDeviceFusionEnabled property of AVCaptureResolvedPhotoSettings.

The default value for this property is true, unless you’re capturing a RAW photo or a bracket using AVCapturePhotoBracketSettings.

Note

When using the deprecated AVCaptureStillImageOutput interface with a virtual device, isAutoVirtualDeviceFusionEnabled is always enabled, if supported.

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

