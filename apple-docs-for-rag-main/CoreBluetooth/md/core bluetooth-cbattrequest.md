

- Core Bluetooth
-  CBATTRequest 

Class

# CBATTRequest

A request that uses the Attribute Protocol (ATT).

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class CBATTRequest
```

## Overview

The CBATTRequest class represents Attribute Protocol (ATT) read and write requests from remote central devices (represented by CBCentral objects). Remote centrals use these ATT requests to read and write characteristic values on local peripherals (represented by CBPeripheralManager objects). Local peripherals, on the other hand, use the properties of CBATTRequest objects to respond to the read and write requests appropriately, using the respond(to:withResult:) method of the CBPeripheralManager class.

## Topics

### Requesting to Read and Write Characteristic Values

var central: CBCentral

The remote central device that originated the request.

var characteristic: CBCharacteristic

The characteristic to read or write the value of.

var value: Data?

The data that the central reads from or writes to the peripheral.

var offset: Int

The zero-based index of the first byte for the read or write request.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Supporting Types

class CBManager

The abstract base class that manages central and peripheral objects.

class CBPeer

An object that represents a remote device.

class CBUUID

A universally unique identifier, as defined by Bluetooth standards.

