

- AVFoundation
- AVCaptureDevice
-  localizedName 

Instance Property

# localizedName

A localized device name for display in the user interface.

iOS 4.0+iPadOS 4.0+Mac Catalyst 14.0+macOS 10.7+tvOS 17.0+visionOS 1.0+

``` source
var localizedName: String { get }
```

## See Also

### Identifying a Device

var uniqueID: String

An identifier that uniquely identifies the device.

var modelID: String

A model identifier for the device.

var manufacturer: String

A human-readable string for the manufacturer of the device.

var deviceType: AVCaptureDevice.DeviceType

The type of device, such as a built-in microphone or wide-angle camera.

struct DeviceType

A structure that defines the device types the framework supports.

var position: AVCaptureDevice.Position

The physical position of the capture device hardware.

enum Position

Constants that indicate the physical position of a capture device.

