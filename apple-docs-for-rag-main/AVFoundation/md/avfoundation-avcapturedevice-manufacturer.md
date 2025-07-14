

- AVFoundation
- AVCaptureDevice
-  manufacturer 

Instance Property

# manufacturer

A human-readable string for the manufacturer of the device.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 10.9+tvOS 17.0+visionOS 2.1+

``` source
var manufacturer: String { get }
```

## Discussion

You can use this property to identify capture devices by manufacturer. For all Apple devices, the value of this property is `Apple Inc.`

Tip

Devices from third-party manufacturers may not provide identifying text, in which case the value of this property is an empty string.

## See Also

### Identifying a Device

var uniqueID: String

An identifier that uniquely identifies the device.

var modelID: String

A model identifier for the device.

var localizedName: String

A localized device name for display in the user interface.

var deviceType: AVCaptureDevice.DeviceType

The type of device, such as a built-in microphone or wide-angle camera.

struct DeviceType

A structure that defines the device types the framework supports.

var position: AVCaptureDevice.Position

The physical position of the capture device hardware.

enum Position

Constants that indicate the physical position of a capture device.

