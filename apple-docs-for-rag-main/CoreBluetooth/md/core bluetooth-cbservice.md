

- Core Bluetooth
-  CBService 

Class

# CBService

A collection of data and associated behaviors that accomplish a function or feature of a device.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class CBService
```

## Overview

CBService objects represent services of a remote peripheral. Services are either primary or secondary and may contain multiple characteristics or included services (references to other services).

## Topics

### Identifying a Service

var peripheral: CBPeripheral?

The peripheral to which this service belongs.

var isPrimary: Bool

A Boolean value that indicates whether the type of service is primary or secondary.

### Accessing Service Data

var characteristics: [CBCharacteristic]?

A list of characteristics discovered in this service.

var includedServices: [CBService]?

A list of included services discovered in this service.

## Relationships

### Inherits From

- CBAttribute

### Inherited By

- CBMutableService

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Services

class CBMutableService

A service with writeable property values.

class CBCharacteristic

A characteristic of a remote peripheral’s service.

class CBMutableCharacteristic

A characteristic of a local peripheral’s service.

class CBDescriptor

An object that provides further information about a remote peripheral’s characteristic.

class CBMutableDescriptor

An object that provides additional information about a local peripheral’s characteristic.

