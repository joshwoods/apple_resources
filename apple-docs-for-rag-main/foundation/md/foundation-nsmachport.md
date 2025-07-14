

- Foundation
-  NSMachPort 

Class

# NSMachPort

A port that can be used as an endpoint for distributed object connections (or raw messaging).

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class NSMachPort
```

## Overview

NSMachPort is a subclass of Port that wraps a Mach port, the fundamental communication port in macOS. NSMachPort allows for local (on the same machine) communication only. A companion class, SocketPort, allows for both local and remote distributed object communication, but may be more expensive than NSMachPort for the local case.

To use NSMachPort effectively, you should be familiar with Mach ports, port access rights, and Mach messages. See the Mach OS documentation for more information.

Note

NSMachPort conforms to the NSCoding protocol, but only supports coding by an NSPortCoder. Port and its subclasses do not support archiving.

## Topics

### Creating and Initializing

class func port(withMachPort: UInt32) -> Port

Creates and returns a port object configured with the given Mach port.

class func port(withMachPort: UInt32, options: NSMachPort.Options) -> Port

Creates and returns a port object configured with the specified options and the given Mach port.

init(machPort: UInt32)

Initializes a newly allocated `NSMachPort` object with a given Mach port.

init(machPort: UInt32, options: NSMachPort.Options)

Initializes a newly allocated `NSMachPort` object with a given Mach port and the specified options.

### Getting the Mach Port

var machPort: UInt32

The Mach port used by the receiver, represented as an integer.

### Scheduling the Port on a Run Loop

func remove(from: RunLoop, forMode: RunLoop.Mode)

Removes the receiver from the run loop mode `mode` of `runLoop`.

func schedule(in: RunLoop, forMode: RunLoop.Mode)

Schedules the receiver into the run loop mode `mode` of `runLoop`.

### Getting and Setting the Delegate

func delegate() -> (any NSMachPortDelegate)?

Returns the receiver’s delegate.

func setDelegate((any NSMachPortDelegate)?)

Sets the receiver’s delegate to a given object.

### Constants

struct Options

Used to remove access rights to a mach port when the `NSMachPort` object is invalidated or destroyed.

## Relationships

### Inherits From

- Port

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol

## See Also

### Legacy

protocol NSMachPortDelegate

An interface for handling incoming Mach messages.

class MessagePort

A port that can be used as an endpoint for distributed object connections (or raw messaging).

protocol PortDelegate

An interface for handling incoming messages.

class PortMessage

A low-level, operating system-independent type for inter-application (and inter-thread) messages.

class NSProtocolChecker

An object that restricts the messages that can be sent to another object (referred to as the checker’s delegate).

