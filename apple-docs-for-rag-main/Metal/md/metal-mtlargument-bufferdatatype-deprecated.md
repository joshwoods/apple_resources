

- Metal
- MTLArgument
-  bufferDataType Deprecated

Instance Property

# bufferDataType

The data type of the buffer data.

iOS 8.0–16.0DeprecatediPadOS 8.0–16.0DeprecatedMac Catalyst 13.1–16.0DeprecatedmacOS 10.11–13.0DeprecatedtvOSDeprecatedvisionOS 1.0–1.0Deprecated

``` source
var bufferDataType: MTLDataType { get }
```

## Discussion

If the argument is not a buffer, querying this property is a fatal error.

## See Also

### Describing a Buffer Argument

var bufferAlignment: Int

The required byte alignment in memory for the buffer data.

Deprecated

var bufferDataSize: Int

The size, in bytes, of the buffer data.

Deprecated

var bufferStructType: MTLStructType?

A description of the structure data of a buffer argument.

Deprecated

var bufferPointerType: MTLPointerType?

A description of the pointer to a buffer argument.

Deprecated

