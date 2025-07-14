

- AVFoundation
- AVCaptureDevice
-  deviceType 

Instance Property

# deviceType

The type of device, such as a built-in microphone or wide-angle camera.

iOS 10.0+iPadOS 10.0+Mac Catalyst 14.0+macOS 10.15+tvOS 17.0+

``` source
var deviceType: AVCaptureDevice.DeviceType { get }
```

## Discussion

Use the default(_:for:position:) method or the AVCaptureDevice.DiscoverySession class to find capture devices by device type.

## See Also

### Identifying a Device

var uniqueID: String

An identifier that uniquely identifies the device.

var modelID: String

A model identifier for the device.

var localizedName: String

A localized device name for display in the user interface.

var manufacturer: String

A human-readable string for the manufacturer of the device.

struct DeviceType

A structure that defines the device types the framework supports.

var position: AVCaptureDevice.Position

The physical position of the capture device hardware.

enum Position

Constants that indicate the physical position of a capture device.

