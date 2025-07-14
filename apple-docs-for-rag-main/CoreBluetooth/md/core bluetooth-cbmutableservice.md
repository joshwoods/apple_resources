

- Core Bluetooth
-  CBMutableService 

Class

# CBMutableService

A service with writeable property values.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class CBMutableService
```

## Overview

The CBMutableService class adds write access to all of the properties in the CBService class it inherits from. You use this class to create a service or an included service on a local peripheral device (represented by a CBPeripheralManager object). After creating a service, you can add it to the peripheral’s local database using the add(_:) method of the CBPeripheralManager class. After you add a service to the peripheral’s local database, Core Bluetooth caches the service and you can no longer make changes to it.

## Topics

### Creating a Mutable Service

init(type: CBUUID, primary: Bool)

Creates a newly initialized mutable service specified by UUID and service type.

### Managing a Mutable Service

var characteristics: [CBCharacteristic]?

A list of characteristics of a service.

var includedServices: [CBService]?

A list of included services.

## Relationships

### Inherits From

- CBService

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

class CBCharacteristic

A characteristic of a remote peripheral’s service.

class CBMutableCharacteristic

A characteristic of a local peripheral’s service.

class CBDescriptor

An object that provides further information about a remote peripheral’s characteristic.

class CBMutableDescriptor

An object that provides additional information about a local peripheral’s characteristic.

