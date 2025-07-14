

- UIKit
- UIImagePickerController
-  isFlashAvailable(for:) 

Type Method

# isFlashAvailable(for:)

Queries whether the specified camera has flash illumination capability.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+

``` source
@MainActor
class func isFlashAvailable(for cameraDevice: UIImagePickerController.CameraDevice) -> Bool
```

## Parameters 

`cameraDevice`  

A UIImagePickerController.CameraDevice constant indicating the camera whose flash capability you want to know.

## Return Value

true if `cameraDevice` can use flash illumination, or false if it cannot.

## See Also

### Related Documentation

var cameraDevice: UIImagePickerController.CameraDevice

The camera used by the image picker controller.

### Configuring the flash behavior

var cameraFlashMode: UIImagePickerController.CameraFlashMode

The flash mode used by the active camera.

enum CameraFlashMode

Constants that specify the flash mode to use with the active camera.

