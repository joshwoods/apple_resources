

- HealthKit
- HKDevice
-  udiDeviceIdentifier 

Instance Property

# udiDeviceIdentifier

The device identifier portion of the US Food and Drug Administration’s Unique Device Identifier (UDI).

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.0+

``` source
var udiDeviceIdentifier: String? { get }
```

## Discussion

The UDI identifies medical devices. You can look up additional information about the device at AccessGUDID. For more information, see FDA Unique Device Identification.

## See Also

### Accessing Data About a Device

var firmwareVersion: String?

An arbitrary string representing the current version of the firmware running on the device.

var hardwareVersion: String?

An arbitrary string representing the hardware version of the device.

var localIdentifier: String?

An identifier that uniquely identifies the device object on the hardware running this code.

var manufacturer: String?

A string representing the device’s manufacturer.

var model: String?

A string representing the device’s model.

var name: String?

The user-facing name for the device.

var softwareVersion: String?

An arbitrary string representing the version of the software running on the device.

