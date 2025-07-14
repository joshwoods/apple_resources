

- Core HID
- HIDDeviceClient
-  HIDDeviceClient.DeviceReference 

Structure

# HIDDeviceClient.DeviceReference

A reference to a HID device on the system.

macOS 15.0+

``` source
struct DeviceReference
```

## Overview

A device reference exists for every discovered device. Use it to create an HIDDeviceClient, and maintain the reference until someone removes the device.

## Topics

### Operators

static func == (HIDDeviceClient.DeviceReference, HIDDeviceClient.DeviceReference) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

let deviceID: UInt64

The unique ID for the associated HID device.

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

CustomStringConvertible Implementations

Equatable Implementations

## Relationships

### Conforms To

- Copyable
- CustomStringConvertible
- Equatable
- Hashable
- Sendable

## See Also

### Create a device client

init?(deviceReference: HIDDeviceClient.DeviceReference)

Creates a client for a HID device.

let deviceReference: HIDDeviceClient.DeviceReference

The reference to the HID device used to create the HID client device.

