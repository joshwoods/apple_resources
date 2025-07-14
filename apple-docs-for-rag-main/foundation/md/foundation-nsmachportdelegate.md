

- Foundation
-  NSMachPortDelegate 

Protocol

# NSMachPortDelegate

An interface for handling incoming Mach messages.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
protocol NSMachPortDelegate : PortDelegate
```

## Overview

Delegates of NSMachPort objects optionally adopt this protocol.

## Topics

### Handling Mach messages

func handleMachMessage(UnsafeMutableRawPointer)

Process an incoming Mach message.

## Relationships

### Inherits From

- NSObjectProtocol
- PortDelegate

## See Also

### Legacy

class NSMachPort

A port that can be used as an endpoint for distributed object connections (or raw messaging).

class MessagePort

A port that can be used as an endpoint for distributed object connections (or raw messaging).

protocol PortDelegate

An interface for handling incoming messages.

class PortMessage

A low-level, operating system-independent type for inter-application (and inter-thread) messages.

class NSProtocolChecker

An object that restricts the messages that can be sent to another object (referred to as the checker’s delegate).

