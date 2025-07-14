

- AVFoundation
- AVCapturePhotoOutput
-  isDualCameraDualPhotoDeliveryEnabled Deprecated

Instance Property

# isDualCameraDualPhotoDeliveryEnabled

A Boolean value that specifies whether to configure the capture pipeline for simultaneous photo capture with both cameras on a dual-camera device.

iOS 11.0–13.0DeprecatediPadOS 11.0–13.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
var isDualCameraDualPhotoDeliveryEnabled: Bool { get set }
```

## Discussion

Enabling this property (on a supported device) allows the capture output to deliver separate images from both the wide-angle and telephoto cameras in a single capture.

Dual photo delivery requires that a capture session set up its internal rendering pipeline differently. If you intend to capture with dual photo delivery at all, set this property to true before calling the AVCaptureSession startRunning() method. Changing this property while the session is running requires a lengthy reconfiguration of the capture render pipeline: Live Photo captures in progress will end immediately, unfulfilled photo requests will abort, and video preview will temporarily freeze.

You must enable this option before initiating a photo capture with the isDualCameraDualPhotoDeliveryEnabled property of your photo settings object set to true. However, after you’ve enabled this option, you are free to issue photo capture requests both with and without dual photo delivery.

## See Also

### Configuring Dual Camera Capture

var isDualCameraFusionSupported: Bool

A Boolean value indicating whether the capture output currently supports automatically combining image data on a dual camera device.

Deprecated

var isDualCameraDualPhotoDeliverySupported: Bool

A Boolean value indicating whether the capture output currently supports simultaneous photo capture with both cameras on a dual-camera device.

Deprecated

