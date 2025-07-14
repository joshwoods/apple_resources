

- Core Bluetooth
-  CBManager 

Class

# CBManager

The abstract base class that manages central and peripheral objects.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.13+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
class CBManager
```

## Topics

### Accessing the Manager’s Properties

var state: CBManagerState

The current state of the manager.

enum CBManagerState

The possible states of a Core Bluetooth manager.

### Determining Authorization State

class var authorization: CBManagerAuthorization

The current authorization status for using Bluetooth.

enum CBManagerAuthorization

The current authorization state of a Core Bluetooth manager.

### Deprecated Properties

var authorization: CBManagerAuthorization

The current authorization status for using Bluetooth.

Deprecated

## Relationships

### Inherits From

- NSObject

### Inherited By

- CBCentralManager
- CBPeripheralManager

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Supporting Types

class CBATTRequest

A request that uses the Attribute Protocol (ATT).

class CBPeer

An object that represents a remote device.

class CBUUID

A universally unique identifier, as defined by Bluetooth standards.

