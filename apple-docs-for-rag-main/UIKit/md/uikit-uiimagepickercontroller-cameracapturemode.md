

- UIKit
- UIImagePickerController
-  cameraCaptureMode 

Instance Property

# cameraCaptureMode

The capture mode used by the camera.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+

``` source
@MainActor
var cameraCaptureMode: UIImagePickerController.CameraCaptureMode { get set }
```

## Discussion

The various capture modes are listed in the UIImagePickerController.CameraCaptureMode enumeration. The default value is UIImagePickerController.CameraCaptureMode.photo.

## See Also

### Related Documentation

var cameraDevice: UIImagePickerController.CameraDevice

The camera used by the image picker controller.

### Configuring the camera capture mode

class func availableCaptureModes(for: UIImagePickerController.CameraDevice) -> [NSNumber]?

Retrieves the capture modes supported by the specified camera device.

enum CameraCaptureMode

Constants that specify the category of media for the camera to capture.

