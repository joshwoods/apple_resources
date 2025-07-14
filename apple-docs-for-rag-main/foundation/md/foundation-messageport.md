

- Foundation
-  MessagePort 

Class

# MessagePort

A port that can be used as an endpoint for distributed object connections (or raw messaging).

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class MessagePort
```

## Overview

MessagePort is a subclass of Port that allows for local (on the same machine) communication only. A companion class, SocketPort, allows for both local and remote communication, but may be more expensive than MessagePort for the local case.

MessagePort defines no additional methods over those already defined by Port.

Note

MessagePort conforms to the NSCoding protocol, but only supports coding by an NSPortCoder object. Port and its subclasses do not support archiving.

Important

Avoid MessagePort. There’s little reason to use MessagePort rather than NSMachPort or SocketPort. There’s no particular performance or functionality advantage. It is recommended avoiding its use.

MessagePort may be deprecated in the macOS 10.6 or later.

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

### Related Documentation

Distributed Objects Programming Topics

### Legacy

protocol NSMachPortDelegate

An interface for handling incoming Mach messages.

class NSMachPort

A port that can be used as an endpoint for distributed object connections (or raw messaging).

protocol PortDelegate

An interface for handling incoming messages.

class PortMessage

A low-level, operating system-independent type for inter-application (and inter-thread) messages.

class NSProtocolChecker

An object that restricts the messages that can be sent to another object (referred to as the checker’s delegate).

