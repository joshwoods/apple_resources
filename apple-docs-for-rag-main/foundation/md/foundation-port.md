

- Foundation
-  Port 

Class

# Port

An abstract class that represents a communication channel.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class Port
```

## Overview

Communication occurs between Port objects, which typically reside in different threads or tasks. The distributed objects system uses Port objects to send PortMessage objects back and forth. Implement interapplication communication using distributed objects whenever possible and use Port objects only when necessary.

To receive incoming messages, add Port objects to an instance of RunLoop as input sources. NSConnection objects automatically add their receive port when initialized.

When the Port object receives a port message, it forwards the message to its delegate in a handleMachMessage(_:) or handle(_:) message. The delegate should implement only one of these methods to process the incoming message in whatever form desired. handleMachMessage(_:) provides a message as a raw Mach message beginning with a `msg_header_t` structure. handle(_:) provides a message as an instance of PortMessage, which is an object-oriented wrapper for a Mach message. If a delegate has not been set, the `NSPort` object handles the message itself.

When you are finished using a port object, you must explicitly invalidate the port object prior to sending it a `release` message. Similarly, if your application uses garbage collection, you must invalidate the port object before removing any strong references to it. If you do not invalidate the port, the resulting port object may linger and create a memory leak. To invalidate the port object, invoke its invalidate() method.

Foundation defines three concrete subclasses of `NSPort`. NSMachPort and MessagePort allow local (on the same machine) communication only. SocketPort allows for both local and remote communication, but may be more expensive than the others for the local case. When creating an `NSPort` object, using doc:nsport/1807189-allocwithzone or port, an NSMachPort object is created instead.

For backward compatibility on Mach, `- [NSPort allocWithZone:]` returns an instance of the NSMachPort class when sent to this class. Otherwise, it returns an instance of a concrete subclass that can be used for messaging between threads or processes on the local machine, or, in the case of SocketPort, between processes on separate machines.

Important

Port conforms to the NSCoding protocol, but only supports coding by an NSPortCoder. Port and its subclasses do not support archiving.

## Topics

### Validation

func invalidate()

Marks the receiver as invalid and posts an didBecomeInvalidNotification to the default notification center.

var isValid: Bool

A Boolean value that indicates whether the receiver is valid.

### Setting the Delegate

func setDelegate((any PortDelegate)?)

Sets the receiver’s delegate to a given object.

func delegate() -> (any PortDelegate)?

Returns the receiver’s delegate.

### Setting Information

func send(before: Date, components: NSMutableArray?, from: Port?, reserved: Int) -> Bool

This method is provided for subclasses that have custom types of `NSPort`.

func send(before: Date, msgid: Int, components: NSMutableArray?, from: Port?, reserved: Int) -> Bool

This method is provided for subclasses that have custom types of `NSPort`.

var reservedSpaceLength: Int

The number of bytes of space reserved by the receiver for sending data.

### Port Monitoring

func remove(from: RunLoop, forMode: RunLoop.Mode)

This method should be implemented by a subclass to stop monitoring of a port when removed from a give run loop in a given input mode.

func schedule(in: RunLoop, forMode: RunLoop.Mode)

This method should be implemented by a subclass to set up monitoring of a port when added to a given run loop in a given input mode.

### Notifications

class let didBecomeInvalidNotification: NSNotification.Name

Posted from the invalidate() method, which is invoked when the `NSPort` is deallocated or when it notices that its communication channel has been damaged. The notification object is the `NSPort` object that has become invalid. This notification does not contain a `userInfo` dictionary.

### Data Types

typealias SocketNativeHandle

Type for the platform-specific native socket handle.

## Relationships

### Inherits From

- NSObject

### Inherited By

- MessagePort
- NSMachPort
- SocketPort

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

### Sockets

class Host

A representation of an individual host on the network.

Deprecated

class SocketPort

A port that represents a BSD socket.

