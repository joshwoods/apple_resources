

- AVFoundation
- AVCaptureDevice
-  uniqueID 

Instance Property

# uniqueID

An identifier that uniquely identifies the device.

iOS 4.0+iPadOS 4.0+Mac Catalyst 14.0+macOS 10.7+tvOS 17.0+visionOS 1.0+

``` source
var uniqueID: String { get }
```

## Discussion

Capture devices have a unique identifier that persists on one system across device connections and disconnections, application restarts, and reboots of the system itself. You can store the value returned by this property to recall or track the status of a specific device in the future.

## See Also

### Identifying a Device

var modelID: String

A model identifier for the device.

var localizedName: String

A localized device name for display in the user interface.

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

