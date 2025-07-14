

- UIKit
- UIImagePickerController
-  availableCaptureModes(for:) 

Type Method

# availableCaptureModes(for:)

Retrieves the capture modes supported by the specified camera device.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+

``` source
@MainActor
class func availableCaptureModes(for cameraDevice: UIImagePickerController.CameraDevice) -> [NSNumber]?
```

## Parameters 

`cameraDevice`  

A UIImagePickerController.CameraDevice constant indicating the camera you want to interrogate.

## Return Value

An array of NSNumber objects indicating the capture modes supported by `cameraDevice`.

## Discussion

See UIImagePickerController.CameraCaptureMode for possible values.

## See Also

### Configuring the camera capture mode

var cameraCaptureMode: UIImagePickerController.CameraCaptureMode

The capture mode used by the camera.

enum CameraCaptureMode

Constants that specify the category of media for the camera to capture.

