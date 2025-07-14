

- Foundation
- OutputStream
-  write(\_:maxLength:) 

Instance Method

# write(\_:maxLength:)

Writes the contents of a provided data buffer to the receiver.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func write(
    _ buffer: UnsafePointer,
    maxLength len: Int
) -> Int
```

## Parameters 

`buffer`  

The data to write.

`len`  

The length of the data buffer, in bytes.

Important

The behavior of this method is undefined if you pass a negative or zero number.

## Return Value

A number indicating the outcome of the operation:

- A positive number indicates the number of bytes written.

- `0` indicates that a fixed-length stream and has reached its capacity.

- `-1` means that the operation failed; more information about the error can be obtained with streamError.

## Mentioned in 

Uploading streams of data

## See Also

### Using Streams

var hasSpaceAvailable: Bool

A boolean value that indicates whether the receiver can be written to.

