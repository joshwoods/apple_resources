

- Metal
- MTLArgument
-  bufferStructType Deprecated

Instance Property

# bufferStructType

A description of the structure data of a buffer argument.

iOS 8.0–16.0DeprecatediPadOS 8.0–16.0DeprecatedMac Catalyst 13.1–16.0DeprecatedmacOS 10.11–13.0DeprecatedtvOSDeprecatedvisionOS 1.0–1.0Deprecated

``` source
var bufferStructType: MTLStructType? { get }
```

## Discussion

If the buffer data type is MTLDataType.struct, this property describes the type of the struct; otherwise, this property is `nil`.

## See Also

### Describing a Buffer Argument

var bufferAlignment: Int

The required byte alignment in memory for the buffer data.

Deprecated

var bufferDataSize: Int

The size, in bytes, of the buffer data.

Deprecated

var bufferDataType: MTLDataType

The data type of the buffer data.

Deprecated

var bufferPointerType: MTLPointerType?

A description of the pointer to a buffer argument.

Deprecated

