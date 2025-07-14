

- Foundation
- DataProtocol
-  copyBytes(to:count:) 

Instance Method

# copyBytes(to:count:)

Copies the provided number of bytes from the start of the type into a typed memory buffer.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@discardableResult
func copyBytes(
    to: UnsafeMutableBufferPointer,
    count: Int
) -> Int
```

**Required** Default implementations provided.

## Parameters 

`to`  

A typed pointer to the buffer you want to copy the bytes into.

`count`  

The number of bytes to copy.

## Return Value

The number of bytes copied.

## Discussion

The following example copies the number of bytes that `count` identified from the beginning of the raw memory buffer into the provided typed memory buffer:

```
let source: [UInt8] = [0, 1, 2]
var dest: [UInt8] = [0xFF, 0xFF, 0xFF, 0xFF, 0xFF, 0xFF]
dest.withUnsafeMutableBufferPointer { typedMemBuffer in
    let count = source.copyBytes(to: typedMemBuffer, count: 1)
    // count == 1
}
// dest = [0x00, 0xFF, 0xFF, 0xFF, 0xFF, 0xFF]

```

## Default Implementations

### DataProtocol Implementations

func copyBytes&lt;DestinationType>(to: UnsafeMutableBufferPointer&lt;DestinationType>, count: Int) -> Int

Copies the provided number of bytes from the start of the type into a typed memory buffer.

func copyBytes(to: UnsafeMutableRawBufferPointer, count: Int) -> Int

Copies the provided number of bytes from the start of the type into a raw memory buffer.

## See Also

### Copying Underlying Bytes

func copyBytes&lt;DestinationType>(to: UnsafeMutableBufferPointer&lt;DestinationType>) -> Int

Copies the bytes of data from the type into a typed memory buffer.

func copyBytes(to: UnsafeMutableRawBufferPointer) -> Int

Copies the bytes of data from the type into a raw memory buffer.

func copyBytes(to: UnsafeMutableRawBufferPointer, count: Int) -> Int

Copies the provided number of bytes from the start of the type into a raw memory buffer.

**Required** Default implementations provided.

func copyBytes&lt;DestinationType, R>(to: UnsafeMutableBufferPointer&lt;DestinationType>, from: R) -> Int

Copies a range of the bytes from the type into a typed memory buffer.

**Required** Default implementations provided.

func copyBytes&lt;R>(to: UnsafeMutableRawBufferPointer, from: R) -> Int

Copies a range of the bytes from the type into a raw memory buffer.

**Required** Default implementations provided.

