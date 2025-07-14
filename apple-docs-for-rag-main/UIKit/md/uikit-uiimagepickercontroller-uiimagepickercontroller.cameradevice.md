

- UIKit
- UIImagePickerController
-  UIImagePickerController.CameraDevice 

Enumeration

# UIImagePickerController.CameraDevice

Constants that specify the camera to use for image or movie capture.

iOSiPadOSMac Catalyst

``` source
enum CameraDevice
```

## Overview

The constants in this enumeration are for use as values of the cameraDevice property.

## Topics

### Constants

case rear

Specifies the camera on the rear of the device.

case front

Specifies the camera on the front of the device.

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

### Configuring the camera to use

class func isCameraDeviceAvailable(UIImagePickerController.CameraDevice) -> Bool

Queries whether the specified camera is available.

var cameraDevice: UIImagePickerController.CameraDevice

The camera used by the image picker controller.

