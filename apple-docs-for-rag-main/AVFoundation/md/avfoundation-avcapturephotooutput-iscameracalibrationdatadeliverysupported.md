

- AVFoundation
- AVCapturePhotoOutput
-  isCameraCalibrationDataDeliverySupported 

Instance Property

# isCameraCalibrationDataDeliverySupported

A Boolean value indicating whether the capture output currently supports delivery of camera calibration data.

iOS 11.0+iPadOS 11.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
var isCameraCalibrationDataDeliverySupported: Bool { get }
```

## Discussion

AVCameraCalibrationData objects describe the imaging parameters of a device camera, and can be useful for performing computer vision tasks in conjunction with dual photo delivery on dual-camera devices.This property’s value can be true only when the isDualCameraDualPhotoDeliveryEnabled property is true. To enable camera calibration delivery, set the isCameraCalibrationDataDeliveryEnabled property in a photo settings object.

This property is key-value observable.

