

- Foundation
- InputStream
-  hasBytesAvailable 

Instance Property

# hasBytesAvailable

A Boolean value that indicates whether the receiver has bytes available to read.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var hasBytesAvailable: Bool { get }
```

## Discussion

true if the receiver has bytes available to read, otherwise false. May also return true if a read must be attempted in order to determine the availability of bytes.

## See Also

### Using Streams

func read(UnsafeMutablePointer&lt;UInt8>, maxLength: Int) -> Int

Reads up to a given number of bytes into a given buffer.

func getBuffer(UnsafeMutablePointer&lt;UnsafeMutablePointer&lt;UInt8>?>, length: UnsafeMutablePointer&lt;Int>) -> Bool

Returns by reference a pointer to a read buffer and, by reference, the number of bytes available, and returns a Boolean value that indicates whether the buffer is available.

