

- AVFoundation
- AVCapturePhoto
-  metadata 

Instance Property

# metadata

A dictionary of metadata describing the captured image.

iOS 11.0+iPadOS 11.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
var metadata: [String : Any] { get }
```

## Discussion

See `CGImageProperties` for possible keys and values. Metadata captured with a photo may include image orientation, EXIF camera properties, and Live Photo metadata.

## See Also

### Accessing Photo Metadata

var depthData: AVDepthData?

Depth or disparity map data captured with the photo.

var cameraCalibrationData: AVCameraCalibrationData?

Calibration information for the camera device that captured the photo.

var sourceDeviceType: AVCaptureDevice.DeviceType?

The type of device that captured the photo.

var portraitEffectsMatte: AVPortraitEffectsMatte?

The portrait effects matte captured with the photo.

