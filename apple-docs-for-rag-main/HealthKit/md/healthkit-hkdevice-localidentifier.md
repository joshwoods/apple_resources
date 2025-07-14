

- HealthKit
- HKDevice
-  localIdentifier 

Instance Property

# localIdentifier

An identifier that uniquely identifies the device object on the hardware running this code.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.0+

``` source
var localIdentifier: String? { get }
```

## Discussion

For example, Bluetooth peripherals that store data directly into HealthKit use the peripheral’s CoreBluetooth UUID. This ID is only valid on the current hardware running the app. For example, connecting the same Bluetooth device to an iPhone and an Apple Watch produces two different local identifiers. Similarly, updating a device changes the local identifier. Device objects with different local identifiers appear as separate devices in the HealthKit Store.

## See Also

### Accessing Data About a Device

var udiDeviceIdentifier: String?

The device identifier portion of the US Food and Drug Administration’s Unique Device Identifier (UDI).

var firmwareVersion: String?

An arbitrary string representing the current version of the firmware running on the device.

var hardwareVersion: String?

An arbitrary string representing the hardware version of the device.

var manufacturer: String?

A string representing the device’s manufacturer.

var model: String?

A string representing the device’s model.

var name: String?

The user-facing name for the device.

var softwareVersion: String?

An arbitrary string representing the version of the software running on the device.

