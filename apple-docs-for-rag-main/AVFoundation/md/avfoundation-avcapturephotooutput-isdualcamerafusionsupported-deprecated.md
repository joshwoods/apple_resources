

- AVFoundation
- AVCapturePhotoOutput
-  isDualCameraFusionSupported Deprecated

Instance Property

# isDualCameraFusionSupported

A Boolean value indicating whether the capture output currently supports automatically combining image data on a dual camera device.

iOS 10.2–13.0DeprecatediPadOS 10.2–13.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
var isDualCameraFusionSupported: Bool { get }
```

## Discussion

On devices equipped with a dual camera, image fusion combines samples from both cameras to produce a higher quality image.

To capture a photo with image fusion, set the isAutoDualCameraFusionEnabled property of your photo settings object. If a device does not support image fusion, setting the isAutoDualCameraFusionEnabled property has no effect (that is, the resolved isDualCameraFusionEnabled setting will always be false).

Note

This property’s value can change if the sessionPreset property of the current capture session or the activeFormat property of the underlying capture device changes.

This property supports key-value observing.

## See Also

### Configuring Dual Camera Capture

var isDualCameraDualPhotoDeliverySupported: Bool

A Boolean value indicating whether the capture output currently supports simultaneous photo capture with both cameras on a dual-camera device.

Deprecated

var isDualCameraDualPhotoDeliveryEnabled: Bool

A Boolean value that specifies whether to configure the capture pipeline for simultaneous photo capture with both cameras on a dual-camera device.

Deprecated

