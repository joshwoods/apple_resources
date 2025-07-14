

- Metal
- MTLVertexAttributeDescriptor
-  format 

Instance Property

# format

The format of the vertex attribute.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
var format: MTLVertexFormat { get set }
```

## Discussion

This property specifies the data type of the vertex attribute that corresponds to an input argument of a shading language function. The MTLVertexFormat may be converted to the data type in the shading function argument with the following specified limitations. Invalid type conversion causes a compilation error.

Conversion of vectors of different lengths is valid. The length of vectors can be reduced. For example, MTLVertexFormat.int4 data can be reduced to a single `int` shader argument is valid, and the last three values of the vector are discarded. Vectors can also be expanded; for example, expanding MTLVertexFormat.int to an `int4` vector shader argument is valid. When expanding, the extra components are filled with the corresponding components of (0,0,0,1).

The sign of an integer MTLVertexFormat can not be cast to a shader argument with an integer type of a different sign. For example, casting the signed format MTLVertexFormat.int to an `uint` shader argument is invalid. Casting MTLVertexFormat.uint to an `int` argument is also invalid.

Integer truncation is not supported. For example, casting the MTLVertexFormat.int to a `short` is invalid. However, casting MTLVertexFormat.short2 to a vector of `int` values is valid.

Casting any MTLVertexFormat to a `float` or `half` is valid. Casting normalized MTLVertexFormat types (such as MTLVertexFormat.short2Normalized) are only valid to `float` or `half`.

## See Also

### Related Documentation

Metal Shading Language Guide

Metal Programming Guide

### Organizing the Vertex Attribute

var offset: Int

The location of an attribute in vertex data, determined by the byte offset from the start of the vertex data.

var bufferIndex: Int

The index in the argument table for the associated vertex buffer.

