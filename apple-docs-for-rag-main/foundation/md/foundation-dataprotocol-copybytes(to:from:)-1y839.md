

- Foundation
- DataProtocol
-  copyBytes(to:from:) 

Instance Method

# copyBytes(to:from:)

Copies a range of the bytes from the type into a raw memory buffer.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@discardableResult
func copyBytes(
    to: UnsafeMutableRawBufferPointer,
    from: R
) -> Int where R : RangeExpression, Self.Index == R.Bound
```

**Required** Default implementations provided.

## Parameters 

`to`  

A pointer to the raw memory buffer you want to copy the bytes into.

`from`  

The range of bytes to copy.

## Return Value

The number of bytes copied.

## Discussion

The following example copies the source bytes that the provided range identifies into the beginning of the specified raw memory buffer:

```
let source: [UInt8] = [0, 1, 2]
var dest: [UInt8] = [0xFF, 0xFF, 0xFF, 0xFF, 0xFF, 0xFF]
_ = dest.withUnsafeMutableBytes { destBufferPtr in
    source.copyBytes(to: destBufferPtr, from: 1...2)
}
// dest = [0x01, 0x02, 0xFF, 0xFF, 0xFF, 0xFF]
```

## Default Implementations

### DataProtocol Implementations

func copyBytes&lt;DestinationType, R>(to: UnsafeMutableBufferPointer&lt;DestinationType>, from: R)

Copies a range of the bytes from the type into a typed memory buffer.

func copyBytes&lt;R>(to: UnsafeMutableRawBufferPointer, from: R) -> Int

Copies a range of the bytes from the type into a raw memory buffer.

func copyBytes&lt;DestinationType, R>(to: UnsafeMutableBufferPointer&lt;DestinationType>, from: R) -> Int

Copies a range of the bytes from the type into a typed memory buffer.

## See Also

### Copying Underlying Bytes

func copyBytes&lt;DestinationType>(to: UnsafeMutableBufferPointer&lt;DestinationType>) -> Int

Copies the bytes of data from the type into a typed memory buffer.

func copyBytes(to: UnsafeMutableRawBufferPointer) -> Int

Copies the bytes of data from the type into a raw memory buffer.

func copyBytes&lt;DestinationType>(to: UnsafeMutableBufferPointer&lt;DestinationType>, count: Int) -> Int

Copies the provided number of bytes from the start of the type into a typed memory buffer.

**Required** Default implementations provided.

func copyBytes(to: UnsafeMutableRawBufferPointer, count: Int) -> Int

Copies the provided number of bytes from the start of the type into a raw memory buffer.

**Required** Default implementations provided.

func copyBytes&lt;DestinationType, R>(to: UnsafeMutableBufferPointer&lt;DestinationType>, from: R) -> Int

Copies a range of the bytes from the type into a typed memory buffer.

**Required** Default implementations provided.

