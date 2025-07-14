

- Foundation
-  PortMessage 

Class

# PortMessage

A low-level, operating system-independent type for inter-application (and inter-thread) messages.

Mac Catalyst 13.0+macOS 10.0+

``` source
class PortMessage
```

## Overview

Port messages are used primarily by the distributed objects system. You should implement inter-application communication using distributed objects whenever possible and use PortMessage only when necessary.

An PortMessage object has three major parts: the send and receive ports, which are Port objects that link the sender of the message to the receiver, and the components, which form the body of the message. The components are held as an NSArray object containing NSData and Port objects. The send(before:) message sends the components out through the send port; any replies to the message arrive on the receive port. See the Port class specification for information on handling incoming messages.

An PortMessage instance can be initialized with a pair of Port objects and an array of components. A port message’s body can contain only Port objects or NSData objects. In the distributed objects system the byte/character arrays are usually encoded NSInvocation objects that are being forwarded from a proxy to the corresponding real object.

An PortMessage object also maintains a message identifier, which can be used to indicate the class of a message, such as an Objective-C method invocation, a connection request, an error, and so on. Use the msgid and msgid methods to access the identifier.

## Topics

### Creating Instances

init(send: Port?, receive: Port?, components: [Any]?)

Initializes a newly allocated `NSPortMessage` object to send given data on a given port and to receiver replies on another given port.

### Sending the Message

func send(before: Date) -> Bool

Attempts to send the message before `aDate`, returning true if successful or false if the operation times out.

### Getting the Components

var components: [Any]?

Returns the data components of the receiver.

### Getting the Ports

var receivePort: Port?

For an outgoing message, returns the port on which replies to the receiver will arrive. For an incoming message, returns the port the receiver did arrive on.

var sendPort: Port?

For an outgoing message, returns the port the receiver will send itself through. For an incoming message, returns the port replies to the receiver should be sent through.

### Accessing the Message ID

var msgid: UInt32

Returns the identifier for the receiver.

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

### Legacy

protocol NSMachPortDelegate

An interface for handling incoming Mach messages.

class NSMachPort

A port that can be used as an endpoint for distributed object connections (or raw messaging).

class MessagePort

A port that can be used as an endpoint for distributed object connections (or raw messaging).

protocol PortDelegate

An interface for handling incoming messages.

class NSProtocolChecker

An object that restricts the messages that can be sent to another object (referred to as the checker’s delegate).

