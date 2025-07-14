

- Foundation
-  InputStream 

Class

# InputStream

A stream that provides read-only stream functionality.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class InputStream
```

## Mentioned in 

Uploading streams of data

## Overview

InputStream is “toll-free bridged” with its Core Foundation counterpart, CFReadStream. For more information on toll-free bridging, see Toll-Free Bridging.

### Subclassing Notes

`NSInputStream` is an abstract superclass of a *class cluster* consisting of concrete subclasses of `NSStream` that provide standard read-only access to stream data. Although `NSInputStream` is probably sufficient for most situations requiring access to stream data, you can create a subclass of `NSInputStream` if you want more specialized behavior (for example, you want to record statistics on the data in a stream).

#### Methods to Override

To create a subclass of `NSInputStream` you may have to implement initializers for the type of stream data supported and suitably re-implement existing initializers. You must also provide complete implementations of the following methods:

- read(_:maxLength:)

From the current read index, take up to the number of bytes specified in the second parameter from the stream and place them in the client-supplied buffer (first parameter). The buffer must be of the size specified by the second parameter. Return the actual number of bytes placed in the buffer; if there is nothing left in the stream, return `0`. Reset the index into the stream for the next read operation.

- getBuffer(_:length:)

Return in 0(1) a pointer to the subclass-allocated buffer (first parameter). Return by reference in the second parameter the number of bytes actually put into the buffer. The buffer’s contents are valid only until the next stream operation. Return false if you cannot access data in the buffer; otherwise, return true. If this method is not appropriate for your type of stream, you may return false.

- hasBytesAvailable

Return true if there is more data to read in the stream, false if there is not. If you want to be semantically compatible with `NSInputStream`, return true if a read must be attempted to determine if bytes are available.

## Topics

### Creating Streams

convenience init?(URL: URL)

Creates and returns an initialized `NSInputStream` object that reads data from the file at a given URL.

init(data: Data)

Initializes and returns an `NSInputStream` object for reading from a given `NSData` object.

convenience init?(fileAtPath: String)

Initializes and returns an `NSInputStream` object that reads data from the file at a given path.

init?(url: URL)

Initializes and returns an `NSInputStream` object that reads data from the file at a given URL.

### Using Streams

func read(UnsafeMutablePointer&lt;UInt8>, maxLength: Int) -> Int

Reads up to a given number of bytes into a given buffer.

func getBuffer(UnsafeMutablePointer&lt;UnsafeMutablePointer&lt;UInt8>?>, length: UnsafeMutablePointer&lt;Int>) -> Bool

Returns by reference a pointer to a read buffer and, by reference, the number of bytes available, and returns a Boolean value that indicates whether the buffer is available.

var hasBytesAvailable: Bool

A Boolean value that indicates whether the receiver has bytes available to read.

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

class OutputStream

A stream that provides write-only stream functionality.

protocol StreamDelegate

An interface that delegates of a stream instance use to handle events on the stream.

