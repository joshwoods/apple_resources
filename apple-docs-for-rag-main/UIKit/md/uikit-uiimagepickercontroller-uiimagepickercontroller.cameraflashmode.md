

- UIKit
- UIImagePickerController
-  UIImagePickerController.CameraFlashMode 

Enumeration

# UIImagePickerController.CameraFlashMode

Constants that specify the flash mode to use with the active camera.

iOSiPadOSMac Catalyst

``` source
enum CameraFlashMode
```

## Overview

The constants in this enumeration are for use as values of the cameraFlashMode property.

The behavior of the flash depends on the camera capture mode.

- For a cameraCaptureMode value of UIImagePickerController.CameraCaptureMode.photo, flash is used to transiently illuminate the subject during still image capture.

- For a cameraCaptureMode value of UIImagePickerController.CameraCaptureMode.video, flash is used to continuously illuminate the subject during movie capture.

For a given camera on a device, flash may or may not be available. You specify the active camera by way of the cameraDevice property. You can determine if the active camera has flash available by calling the isFlashAvailable(for:) class method.

You can manipulate the flash directly to provide effects such as a strobe light. Present a picker interface set to use video capture mode. Then, turn the flash LED on or off by setting the cameraFlashMode property to UIImagePickerController.CameraFlashMode.on or UIImagePickerController.CameraFlashMode.off.

## Topics

### Constants

case off

Specifies that flash illumination is always off, no matter what the ambient light conditions are.

case auto

Specifies that the device should consider ambient light conditions to automatically determine whether or not to use flash illumination.

case on

Specifies that flash illumination is always on, no matter what the ambient light conditions are.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Configuring the flash behavior

class func isFlashAvailable(for: UIImagePickerController.CameraDevice) -> Bool

Queries whether the specified camera has flash illumination capability.

var cameraFlashMode: UIImagePickerController.CameraFlashMode

The flash mode used by the active camera.

