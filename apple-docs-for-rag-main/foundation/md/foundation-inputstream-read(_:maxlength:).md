

- Foundation
- InputStream
-  read(\_:maxLength:) 

Instance Method

# read(\_:maxLength:)

Reads up to a given number of bytes into a given buffer.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func read(
    _ buffer: UnsafeMutablePointer,
    maxLength len: Int
) -> Int
```

## Parameters 

`buffer`  

A data buffer. The buffer must be large enough to contain the number of bytes specified by `len`.

`len`  

The maximum number of bytes to read.

## Return Value

A number indicating the outcome of the operation:

## Discussion

- A positive number indicates the number of bytes read.

- `0` indicates that the end of the buffer was reached.

- `-1` means that the operation failed; more information about the error can be obtained with streamError.

## See Also

### Using Streams

func getBuffer(UnsafeMutablePointer&lt;UnsafeMutablePointer&lt;UInt8>?>, length: UnsafeMutablePointer&lt;Int>) -> Bool

Returns by reference a pointer to a read buffer and, by reference, the number of bytes available, and returns a Boolean value that indicates whether the buffer is available.

var hasBytesAvailable: Bool

A Boolean value that indicates whether the receiver has bytes available to read.

