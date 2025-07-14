

- Metal
- MTLArgument
-  bufferAlignment Deprecated

Instance Property

# bufferAlignment

The required byte alignment in memory for the buffer data.

iOS 8.0–16.0DeprecatediPadOS 8.0–16.0DeprecatedMac Catalyst 13.1–16.0DeprecatedmacOS 10.11–13.0DeprecatedtvOSDeprecatedvisionOS 1.0–1.0Deprecated

``` source
var bufferAlignment: Int { get }
```

## Discussion

If the argument is not a buffer, querying this property is a fatal error.

## See Also

### Describing a Buffer Argument

var bufferDataSize: Int

The size, in bytes, of the buffer data.

Deprecated

var bufferDataType: MTLDataType

The data type of the buffer data.

Deprecated

var bufferStructType: MTLStructType?

A description of the structure data of a buffer argument.

Deprecated

var bufferPointerType: MTLPointerType?

A description of the pointer to a buffer argument.

Deprecated

