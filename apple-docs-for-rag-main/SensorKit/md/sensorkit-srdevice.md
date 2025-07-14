

- SensorKit
-  SRDevice 

Class

# SRDevice

A representation of a device that provides sample data.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
class SRDevice
```

## Overview

This class supports iOS and watchOS devices.

## Topics

### Accessing Device Information

var model: String

The user-defined name of the device.

var name: String

The framework-defined name of the device.

var systemName: String

The device’s operating system.

var systemVersion: String

The device’s operating system version.

var productType: String

A string that identifies the device used to save a sample.

### Accessing the Primary Device

class var current: SRDevice

The device that runs the app.

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

## See Also

### Selecting the Device

var device: SRDevice

The device to query for sample data.

