

- Foundation
-  OutputStream 

Class

# OutputStream

A stream that provides write-only stream functionality.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class OutputStream
```

## Mentioned in 

Uploading streams of data

## Overview

OutputStream is “toll-free bridged” with its Core Foundation counterpart, CFWriteStream. For more information on toll-free bridging, see Toll-Free Bridging.

### Subclassing Notes

`NSOutputStream` is a concrete subclass of `NSStream` that lets you write data to a stream. Although `NSOutputStream` is probably sufficient for most situations requiring this capability, you can create a subclass of `NSOutputStream` if you want more specialized behavior (for example, you want to record statistics on the data in a stream).

#### Methods to Override

To create a subclass of `NSOutputStream` you may have to implement initializers for the type of stream data supported and suitably reimplement existing initializers. You must also provide complete implementations of the following methods:

- write(_:maxLength:)

From the current write pointer, take up to the number of bytes specified in the `maxLength:` parameter from the client-supplied buffer (first parameter) and put them onto the stream. The buffer must be of the size specified by the second parameter. To prepare for the next operation, offset the write pointer by the number of bytes written. Return a signed integer based on the outcome of the current operation:

- If the write operation is successful, return the actual number of bytes put onto the stream.

- If the stream is of a fixed length and has reached its capacity, return `0`.

- If there was an error writing to the stream, return `-1`.

- hasSpaceAvailable

Return true if the stream can currently accept more data, false if it cannot. If you want to be semantically compatible with `NSOutputStream`, return true if a write must be attempted to determine if space is available.

## Topics

### Creating Streams

class func toMemory() -> Self

Creates and returns an initialized output stream that will write stream data to memory.

convenience init?(URL: URL, append: Bool)

Creates and returns an initialized output stream for writing to a specified URL.

init(toMemory: ())

Returns an initialized output stream that will write to memory.

init(toBuffer: UnsafeMutablePointer&lt;UInt8>, capacity: Int)

Returns an initialized output stream that can write to a provided buffer.

convenience init?(toFileAtPath: String, append: Bool)

Returns an initialized output stream for writing to a specified file.

init?(url: URL, append: Bool)

Returns an initialized output stream for writing to a specified URL.

### Using Streams

var hasSpaceAvailable: Bool

A boolean value that indicates whether the receiver can be written to.

func write(UnsafePointer&lt;UInt8>, maxLength: Int) -> Int

Writes the contents of a provided data buffer to the receiver.

## Relationships

### Inherits From

- Stream

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Streams

class Stream

An abstract class representing a stream.

class InputStream

A stream that provides read-only stream functionality.

protocol StreamDelegate

An interface that delegates of a stream instance use to handle events on the stream.

