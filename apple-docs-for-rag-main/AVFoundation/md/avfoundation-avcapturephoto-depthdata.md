

- AVFoundation
- AVCapturePhoto
-  depthData 

Instance Property

# depthData

Depth or disparity map data captured with the photo.

iOS 11.0+iPadOS 11.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
var depthData: AVDepthData? { get }
```

## Mentioned in 

Capturing Photos with Depth

## Discussion

To request capture of depth data alongside a photo (on supported devices), set the isDepthDataDeliveryEnabled property of your photo settings object to true when requesting photo capture. If you did not request depth data delivery, this property’s value is `nil`.

Note

If you set the embedsDepthDataInPhoto property of your photo object to false when requesting photo capture, this property still provides depth data, but that data is not included when generating photo file data for output.

## See Also

### Accessing Photo Metadata

var cameraCalibrationData: AVCameraCalibrationData?

Calibration information for the camera device that captured the photo.

var sourceDeviceType: AVCaptureDevice.DeviceType?

The type of device that captured the photo.

var metadata: [String : Any]

A dictionary of metadata describing the captured image.

var portraitEffectsMatte: AVPortraitEffectsMatte?

The portrait effects matte captured with the photo.

