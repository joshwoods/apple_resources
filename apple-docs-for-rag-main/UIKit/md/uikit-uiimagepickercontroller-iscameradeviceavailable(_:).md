

- UIKit
- UIImagePickerController
-  isCameraDeviceAvailable(\_:) 

Type Method

# isCameraDeviceAvailable(\_:)

Queries whether the specified camera is available.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+

``` source
@MainActor
class func isCameraDeviceAvailable(_ cameraDevice: UIImagePickerController.CameraDevice) -> Bool
```

## Parameters 

`cameraDevice`  

A UIImagePickerController.CameraDevice constant indicating the camera whose availability you want to check.

## Return Value

true if the camera indicated by `cameraDevice` is available, or false if it is not available.

## See Also

### Related Documentation

class func isFlashAvailable(for: UIImagePickerController.CameraDevice) -> Bool

Queries whether the specified camera has flash illumination capability.

class func availableCaptureModes(for: UIImagePickerController.CameraDevice) -> [NSNumber]?

Retrieves the capture modes supported by the specified camera device.

### Configuring the camera to use

var cameraDevice: UIImagePickerController.CameraDevice

The camera used by the image picker controller.

enum CameraDevice

Constants that specify the camera to use for image or movie capture.

