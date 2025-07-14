

- UIKit
- UIImagePickerController
-  cameraDevice 

Instance Property

# cameraDevice

The camera used by the image picker controller.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+

``` source
@MainActor
var cameraDevice: UIImagePickerController.CameraDevice { get set }
```

## Discussion

The default is UIImagePickerController.CameraDevice.rear.

## See Also

### Related Documentation

class func isFlashAvailable(for: UIImagePickerController.CameraDevice) -> Bool

Queries whether the specified camera has flash illumination capability.

class func availableCaptureModes(for: UIImagePickerController.CameraDevice) -> [NSNumber]?

Retrieves the capture modes supported by the specified camera device.

### Configuring the camera to use

class func isCameraDeviceAvailable(UIImagePickerController.CameraDevice) -> Bool

Queries whether the specified camera is available.

enum CameraDevice

Constants that specify the camera to use for image or movie capture.

