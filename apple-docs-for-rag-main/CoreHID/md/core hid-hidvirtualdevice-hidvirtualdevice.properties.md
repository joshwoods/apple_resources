

- Core HID
- HIDVirtualDevice
-  HIDVirtualDevice.Properties 

Structure

# HIDVirtualDevice.Properties

The properties for a virtual HID device.

macOS 15.0+

``` source
struct Properties
```

## Mentioned in 

Creating virtual devices

## Overview

A virtual device has many properties, required and optional, that determine or alter its functionality. Use this class to provide these properties during the creation of a virtual device.

Uncommon properties that aren’t available can be specified in the `extraProperties` parameter of init(descriptor:vendorID:productID:transport:product:manufacturer:modelNumber:versionNumber:serialNumber:uniqueID:locationID:localizationCode:extraProperties:).

## Topics

### Initializers

init(descriptor: Data, vendorID: UInt32, productID: UInt32?, transport: HIDDeviceTransport?, product: String?, manufacturer: String?, modelNumber: String?, versionNumber: UInt64?, serialNumber: String?, uniqueID: String?, locationID: UInt64?, localizationCode: HIDDeviceLocalizationCode?, extraProperties: Dictionary&lt;String, AnyObject>?)

Creates a set of properties for a virtual device.

### Instance Properties

let descriptor: Data

The HID specification compliant report descriptor for the virtual device.

let localizationCode: HIDDeviceLocalizationCode?

A device localization code that specifies the HID compliant localization code.

let locationID: UInt64?

The location ID for the device.

let manufacturer: String?

The manufacturer of the device.

let modelNumber: String?

The model number for the device.

let product: String?

The product name for the device.

let productID: UInt32?

The product ID for the device.

let serialNumber: String?

The serial number for the device.

let transport: HIDDeviceTransport?

The data transport for the device.

let uniqueID: String?

A unique ID for the device.

let vendorID: UInt32

The vendor ID for the device.

let versionNumber: UInt64?

The version of the device.

## Relationships

### Conforms To

- Sendable

## See Also

### Simulation

Creating virtual devices

Use and interact with a virtual human interface device for testing and development.

actor HIDVirtualDevice

A virtual service to emulate a HID device connected to the system.

protocol HIDVirtualDeviceDelegate

The delegate to receive notifications for a virtual HID device.

