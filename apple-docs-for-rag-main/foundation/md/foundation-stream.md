

- Foundation
-  Stream 

Class

# Stream

An abstract class representing a stream.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class Stream
```

## Mentioned in 

Uploading streams of data

## Overview

This class’s interface is common to all Cocoa stream classes, including its concrete subclasses InputStream and OutputStream.

Stream objects provide an easy way to read and write data to and from a variety of media in a device-independent way. You can create stream objects for data located in memory, in a file, or on a network (using sockets), and you can use stream objects without loading all of the data into memory at once.

By default, Stream instances that aren’t file-based are non-seekable, one-way streams (although custom seekable subclasses are possible). After you provide or consume data, you can’t retrieve the data from the stream.

### Subclassing Notes

Stream is an abstract class, incapable of instantiation and intended for you to subclass it. It publishes a programmatic interface that all subclasses must adopt and provide implementations for. The two Apple-provided concrete subclasses of Stream, InputStream and OutputStream, are suitable for most purposes. However, there might be situations when you want a peer subclass to InputStream and OutputStream. For example, you might want a class that implements a full-duplex (two-way) stream, or a class whose instances are capable of seeking through a stream.

#### Methods to Override

All subclasses must fully implement the following methods:

- open() and close()

Implement open() to open the stream for reading or writing and make the stream available to the client directly or, if the stream object is scheduled on a run loop, to the delegate. Implement close() to close the stream and remove the stream object from the run loop, if necessary. A closed stream should still be able to accept new properties and report its current properties. Once you close a stream, you can’t reopen it.

- delegate

Return and set the delegate. By a default, a stream object must be its own delegate; so a delegate message with an argument of `nil` should restore this delegate. Don’t retain the delegate to prevent retain cycles.

To learn about delegates and delegation, read “Delegation” in Cocoa Fundamentals Guide.

- schedule(in:forMode:) and remove(from:forMode:)

Implement schedule(in:forMode:) to schedule the stream object on the specified run loop for the specified mode. Implement remove(from:forMode:) to remove the object from the run loop. See the documentation of the RunLoop class for details. Once the stream object for an open stream is scheduled on a run loop, it is the responsibility of the subclass as it processes stream data to send stream(_:handle:) messages to its delegate.

- property(forKey:) and setProperty(_:forKey:)

Implement these methods to return and set, respectively, the property value for the specified key. You may add custom properties, but be sure to handle all properties defined by Stream as well.

- streamStatus and streamError

Implement streamStatus to return the current status of the stream as a Stream.Status constant; you may define new Stream.Status constants, but be sure to handle the system defined constants properly. Implement streamError to return an NSError object representing the current error. You might decide to return a custom NSError object that can provide complete and localized information about the error.

## Topics

### Creating Streams

class func getStreamsTo(Host, port: Int, inputStream: AutoreleasingUnsafeMutablePointer&lt;InputStream?>?, outputStream: AutoreleasingUnsafeMutablePointer&lt;OutputStream?>?)

Creates and returns by reference an `NSInputStream` object and `NSOutputStream` object for a socket connection with a given host on a given port.

Deprecated

### Configuring Streams

func property(forKey: Stream.PropertyKey) -> Any?

Returns the receiver’s property for a given key.

func setProperty(Any?, forKey: Stream.PropertyKey) -> Bool

Attempts to set the value of a given property of the receiver and returns a Boolean value that indicates whether the value is accepted by the receiver.

var delegate: (any StreamDelegate)?

Sets the receiver’s delegate.

### Using Streams

func open()

Opens the receiving stream.

func close()

Closes the receiver.

### Managing Run Loops

func schedule(in: RunLoop, forMode: RunLoop.Mode)

Schedules the receiver on a given run loop in a given mode.

func remove(from: RunLoop, forMode: RunLoop.Mode)

Removes the receiver from a given run loop running in a given mode.

### Getting Stream Information

var streamStatus: Stream.Status

Returns the receiver’s status.

var streamError: (any Error)?

Returns an `NSError` object representing the stream error.

### Constants

enum Status

The type declared for the constants listed in doc:stream/stream_status_constants.

Stream Status Constants

These constants indicate the current status of a stream. They are returned by streamStatus.

struct Event

Describes the constants that may be sent to the delegate as a bit field in the second parameter of stream(_:handle:) to specify the kind of stream event.

struct StreamNetworkServiceTypeValue

`NSStream` defines these string constants for specifying the service type of a stream.

struct StreamSOCKSProxyConfiguration

struct StreamSOCKSProxyVersion

struct StreamSocketSecurityLevel

`NSStream` defines these string constants for specifying the secure-socket layer (SSL) security level.

struct PropertyKey

`NSStream` defines these string constants as keys for accessing stream properties using property(forKey:) and setting properties with setProperty(_:forKey:):

let NSStreamSocketSSLErrorDomain: String

The error domain used by `NSError` when reporting SSL errors.

let NSStreamSOCKSErrorDomain: String

The error domain used by `NSError` when reporting SOCKS errors.

### Type Methods

class func getBoundStreams(withBufferSize: Int, inputStream: AutoreleasingUnsafeMutablePointer&lt;InputStream?>?, outputStream: AutoreleasingUnsafeMutablePointer&lt;OutputStream?>?)

Creates and returns by reference a bound pair of input and output streams.

class func getStreamsToHost(withName: String, port: Int, inputStream: AutoreleasingUnsafeMutablePointer&lt;InputStream?>?, outputStream: AutoreleasingUnsafeMutablePointer&lt;OutputStream?>?)Deprecated

## Relationships

### Inherits From

- NSObject

### Inherited By

- InputStream
- OutputStream

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Streams

class InputStream

A stream that provides read-only stream functionality.

class OutputStream

A stream that provides write-only stream functionality.

protocol StreamDelegate

An interface that delegates of a stream instance use to handle events on the stream.

