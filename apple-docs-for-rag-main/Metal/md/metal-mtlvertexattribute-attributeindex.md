

- Metal
- MTLVertexAttribute
-  attributeIndex 

Instance Property

# attributeIndex

The index of the attribute, as declared in Metal shader source code.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
var attributeIndex: Int { get }
```

## See Also

### Describing the Attribute

var name: String

The name of the attribute.

var attributeType: MTLDataType

The data type for the attribute, as declared in Metal shader source code.

var isActive: Bool

A Boolean value that indicates whether this vertex attribute is active.

var isPatchControlPointData: Bool

A Boolean value that indicates whether this vertex attribute represents control point data.

var isPatchData: Bool

A Boolean value that indicates whether this vertex attribute represents patch data.

