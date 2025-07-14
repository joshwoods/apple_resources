

- AVFoundation
- AVCapturePhotoOutput
-  isDualCameraDualPhotoDeliverySupported Deprecated

Instance Property

# isDualCameraDualPhotoDeliverySupported

A Boolean value indicating whether the capture output currently supports simultaneous photo capture with both cameras on a dual-camera device.

iOS 11.0–13.0DeprecatediPadOS 11.0–13.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
var isDualCameraDualPhotoDeliverySupported: Bool { get }
```

## Discussion

Not all devices and capture formats support dual camera capture. This property’s value can change if the sessionPreset property of the current capture session or the activeFormat property of the underlying capture device changes. If a camera or format change causes this property’s value to become false, the isDualCameraDualPhotoDeliveryEnabled property’s value also becomes false.

This property is key-value observable.

## See Also

### Configuring Dual Camera Capture

var isDualCameraFusionSupported: Bool

A Boolean value indicating whether the capture output currently supports automatically combining image data on a dual camera device.

Deprecated

var isDualCameraDualPhotoDeliveryEnabled: Bool

A Boolean value that specifies whether to configure the capture pipeline for simultaneous photo capture with both cameras on a dual-camera device.

Deprecated

