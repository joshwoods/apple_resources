

- AVFoundation
- AVCapturePhoto
-  sourceDeviceType 

Instance Property

# sourceDeviceType

The type of device that captured the photo.

iOS 11.0+iPadOS 11.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
var sourceDeviceType: AVCaptureDevice.DeviceType? { get }
```

## Discussion

When you capture dual photos with a builtInDualCamera device and the isDualCameraDualPhotoDeliveryEnabled setting, use this property to determine which of the two resulting photo objects is from the builtInWideAngleCamera or builtInTelephotoCamera device.

For all other captures, this property’s value is equal to the deviceType property of the capture device to which the photo output is connected.

This property’s value can be `nil` if the AVCapturePhoto object did not come from an AVCaptureDevice capture.

## See Also

### Accessing Photo Metadata

var depthData: AVDepthData?

Depth or disparity map data captured with the photo.

var cameraCalibrationData: AVCameraCalibrationData?

Calibration information for the camera device that captured the photo.

var metadata: [String : Any]

A dictionary of metadata describing the captured image.

var portraitEffectsMatte: AVPortraitEffectsMatte?

The portrait effects matte captured with the photo.

