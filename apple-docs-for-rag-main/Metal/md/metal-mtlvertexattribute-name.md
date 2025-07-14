

- Metal
- MTLVertexAttribute
-  name 

Instance Property

# name

The name of the attribute.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
var name: String { get }
```

## See Also

### Related Documentation

Metal Shading Language Guide

Metal Programming Guide

### Describing the Attribute

var attributeIndex: Int

The index of the attribute, as declared in Metal shader source code.

var attributeType: MTLDataType

The data type for the attribute, as declared in Metal shader source code.

var isActive: Bool

A Boolean value that indicates whether this vertex attribute is active.

var isPatchControlPointData: Bool

A Boolean value that indicates whether this vertex attribute represents control point data.

var isPatchData: Bool

A Boolean value that indicates whether this vertex attribute represents patch data.

