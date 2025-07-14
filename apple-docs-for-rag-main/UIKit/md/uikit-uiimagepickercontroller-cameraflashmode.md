

- UIKit
- UIImagePickerController
-  cameraFlashMode 

Instance Property

# cameraFlashMode

The flash mode used by the active camera.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+

``` source
@MainActor
var cameraFlashMode: UIImagePickerController.CameraFlashMode { get set }
```

## Discussion

The various flash modes are listed in the UIImagePickerController.CameraFlashMode enumeration. The default value is UIImagePickerController.CameraFlashMode.auto.

The value of this property specifies the behavior of the still-image flash when the value of the cameraCaptureMode property is UIImagePickerController.CameraCaptureMode.photo, and specifies the behavior of the video torch when cameraCaptureMode is UIImagePickerController.CameraCaptureMode.video.

## See Also

### Related Documentation

var cameraDevice: UIImagePickerController.CameraDevice

The camera used by the image picker controller.

var cameraCaptureMode: UIImagePickerController.CameraCaptureMode

The capture mode used by the camera.

### Configuring the flash behavior

class func isFlashAvailable(for: UIImagePickerController.CameraDevice) -> Bool

Queries whether the specified camera has flash illumination capability.

enum CameraFlashMode

Constants that specify the flash mode to use with the active camera.

