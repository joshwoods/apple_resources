

- Foundation
- InputStream
-  getBuffer(\_:length:) 

Instance Method

# getBuffer(\_:length:)

Returns by reference a pointer to a read buffer and, by reference, the number of bytes available, and returns a Boolean value that indicates whether the buffer is available.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func getBuffer(
    _ buffer: UnsafeMutablePointer?>,
    length len: UnsafeMutablePointer
) -> Bool
```

## Parameters 

`buffer`  

Upon return, contains a pointer to a read buffer. The buffer is only valid until the next stream operation is performed.

`len`  

Upon return, contains the number of bytes available.

## Return Value

true if the buffer is available, otherwise false.

## Discussion

Subclasses of `NSInputStream` may return false if this operation is not appropriate for the stream type.

## See Also

### Using Streams

func read(UnsafeMutablePointer&lt;UInt8>, maxLength: Int) -> Int

Reads up to a given number of bytes into a given buffer.

var hasBytesAvailable: Bool

A Boolean value that indicates whether the receiver has bytes available to read.

