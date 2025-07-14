

- Core Bluetooth
-  CBMutableCharacteristic 

Class

# CBMutableCharacteristic

A characteristic of a local peripheral’s service.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class CBMutableCharacteristic
```

## Overview

CBMutableCharacteristic objects represent the characteristics of a local peripheral’s service. This class adds write access to many of the properties in the CBCharacteristic class, which it inherits from.

You use this class to create a characteristic and to set its properties and permissions as desired. After you create and add a characteristic to a local service, you can publish it (and the service) to the peripheral’s local database with the add(_:) method of the CBPeripheralManager class. After you publish a characteristic, Core Bluetooth caches the characteristic and you can’t make changes to it.

## Topics

### Creating a Mutable Characteristic

init(type: CBUUID, properties: CBCharacteristicProperties, value: Data?, permissions: CBAttributePermissions)

Creates a mutable characteristic with specified permissions, properties, and value.

### Managing a Mutable Characteristic

var value: Data?

The value of the characteristic.

var descriptors: [CBDescriptor]?

An array of the characteristic’s descriptors.

var properties: CBCharacteristicProperties

The properties of the characteristic.

var permissions: CBAttributePermissions

The permissions of the characteristic value.

struct CBAttributePermissions

Values that represent the read, write, and encryption permissions for a characteristic’s value.

var subscribedCentrals: [CBCentral]?

A list of centrals that are currently subscribed to the characteristic’s value.

## Relationships

### Inherits From

- CBCharacteristic

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Services

class CBService

A collection of data and associated behaviors that accomplish a function or feature of a device.

class CBMutableService

A service with writeable property values.

class CBCharacteristic

A characteristic of a remote peripheral’s service.

class CBDescriptor

An object that provides further information about a remote peripheral’s characteristic.

class CBMutableDescriptor

An object that provides additional information about a local peripheral’s characteristic.

