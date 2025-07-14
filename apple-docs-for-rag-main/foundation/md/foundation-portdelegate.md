

- Foundation
-  PortDelegate 

Protocol

# PortDelegate

An interface for handling incoming messages.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
protocol PortDelegate : NSObjectProtocol
```

## Overview

The PortDelegate protocol defines the optional methods implemented by delegates of Port objects.

## Topics

### Handling Port Messages

func handle(NSPortMessage)

Processes a given incoming message on the port.

## Relationships

### Inherits From

- NSObjectProtocol

### Inherited By

- NSMachPortDelegate

## See Also

### Legacy

protocol NSMachPortDelegate

An interface for handling incoming Mach messages.

class NSMachPort

A port that can be used as an endpoint for distributed object connections (or raw messaging).

class MessagePort

A port that can be used as an endpoint for distributed object connections (or raw messaging).

class PortMessage

A low-level, operating system-independent type for inter-application (and inter-thread) messages.

class NSProtocolChecker

An object that restricts the messages that can be sent to another object (referred to as the checker’s delegate).

