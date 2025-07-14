

- HealthKit
-  HKDevice 

Class

# HKDevice

A device that generates data for HealthKit.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.0+

``` source
class HKDevice
```

## Mentioned in 

About the HealthKit framework

## Overview

Devices include Apple Watch, iPhone, and any other health or fitness peripherals that produce the sample data stored in HealthKit. Device objects are immutable: You set the device’s properties when you create the HKDevice object, and they cannot change.

## Topics

### Creating Device Objects

init(name: String?, manufacturer: String?, model: String?, hardwareVersion: String?, firmwareVersion: String?, softwareVersion: String?, localIdentifier: String?, udiDeviceIdentifier: String?)

Initializes a new device object.

class func local() -> HKDevice

returns a device object that represents the current device.

### Accessing Data About a Device

var udiDeviceIdentifier: String?

The device identifier portion of the US Food and Drug Administration’s Unique Device Identifier (UDI).

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

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding
- Sendable

## See Also

### Sources and devices

struct HKSourceQueryDescriptor

A query interface that uses Swift concurrency to read the apps and devices that produced the matching samples.

class HKSourceRevision

An object indicating the source of a HealthKit sample.

class HKSource

An object indicating the app or device that created a HealthKit sample

class HKSourceQuery

A query that returns a list of sources, such as apps and devices, that have saved matching queries to the HealthKit store.

