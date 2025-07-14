

- Core Bluetooth
-  CBDescriptor 

Class

# CBDescriptor

An object that provides further information about a remote peripheral’s characteristic.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class CBDescriptor
```

## Overview

CBDescriptor and its subclass CBMutableDescriptor represent a descriptor of a peripheral’s characteristic. In partcular, CBDescriptor objects represent the descriptors of a remote peripheral’s characteristic. Descriptors provide further information about a characteristic’s value. For example, they may describe the value in human-readable form and describe how to format the value for presentation purposes. Characteristic descriptors also indicate whether a characteristic’s value indicates or notifies a client (a central) when the value of the characteristic changes.

CBUUID details six predefined descriptors and their corresponding value types. CBDescriptor lists the predefined descriptors and the CBUUID constants that represent them.

| Descriptor type | Descriptor constant |
|----|----|
| Characteristic extended properties | CBUUIDCharacteristicExtendedPropertiesString |
| Characteristic user description | CBUUIDCharacteristicUserDescriptionString |
| Client characteristic configuration | CBUUIDClientCharacteristicConfigurationString |
| Server characteristic configuration | CBUUIDServerCharacteristicConfigurationString |
| Characteristic format | CBUUIDCharacteristicFormatString |
| Characteristic aggregate format | CBUUIDCharacteristicAggregateFormatString |

## Topics

### Identifying a Descriptor

var characteristic: CBCharacteristic?

The characteristic to which this descriptor belongs.

### Accessing Descriptor Data

var value: Any?

The value of the descriptor.

## Relationships

### Inherits From

- CBAttribute

### Inherited By

- CBMutableDescriptor

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

class CBMutableCharacteristic

A characteristic of a local peripheral’s service.

class CBMutableDescriptor

An object that provides additional information about a local peripheral’s characteristic.

