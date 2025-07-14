

- Core Bluetooth
-  CBCentral 

Class

# CBCentral

A remote device connected to a local app, which is acting as a peripheral.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class CBCentral
```

## Overview

The CBCentral class represents remote central devices (or *centrals*) that have connected to an app implementing the peripheral role on a local device. Remote centrals use universally unique identifiers (UUIDs), represented by NSUUID objects, to identify themselves.

## Topics

### Identifying a Remote Central

var maximumUpdateValueLength: Int

The maximum amount of data, in bytes, that the central can receive in a single notification or indication.

## Relationships

### Inherits From

- CBPeer

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Centrals

class CBCentralManager

An object that scans for, discovers, connects to, and manages peripherals.

protocol CBCentralManagerDelegate

A protocol that provides updates for the discovery and management of peripheral devices.

