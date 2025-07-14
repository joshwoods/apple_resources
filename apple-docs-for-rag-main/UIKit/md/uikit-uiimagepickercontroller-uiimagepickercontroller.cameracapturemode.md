

- UIKit
- UIImagePickerController
-  UIImagePickerController.CameraCaptureMode 

Enumeration

# UIImagePickerController.CameraCaptureMode

Constants that specify the category of media for the camera to capture.

iOSiPadOSMac Catalyst

``` source
enum CameraCaptureMode
```

## Overview

The constants in this enumeration are for use as values of the cameraCaptureMode property.

## Topics

### Constants

case photo

Specifies that the camera captures still images.

case video

Specifies that the camera captures movies.

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

### Configuring the camera capture mode

class func availableCaptureModes(for: UIImagePickerController.CameraDevice) -> [NSNumber]?

Retrieves the capture modes supported by the specified camera device.

var cameraCaptureMode: UIImagePickerController.CameraCaptureMode

The capture mode used by the camera.

