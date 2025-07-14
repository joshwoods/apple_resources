

- AVFoundation
- AVCapturePhoto
-  cameraCalibrationData 

Instance Property

# cameraCalibrationData

Calibration information for the camera device that captured the photo.

iOS 11.0+iPadOS 11.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
var cameraCalibrationData: AVCameraCalibrationData? { get }
```

## Discussion

Camera calibration data is present only if you specified the isCameraCalibrationDataDeliveryEnabled and isDualCameraDualPhotoDeliveryEnabled settings when requesting capture. For camera calibration data in a capture that includes depth data, see the AVDepthData cameraCalibrationData property.

## See Also

### Accessing Photo Metadata

var depthData: AVDepthData?

Depth or disparity map data captured with the photo.

var sourceDeviceType: AVCaptureDevice.DeviceType?

The type of device that captured the photo.

var metadata: [String : Any]

A dictionary of metadata describing the captured image.

var portraitEffectsMatte: AVPortraitEffectsMatte?

The portrait effects matte captured with the photo.

