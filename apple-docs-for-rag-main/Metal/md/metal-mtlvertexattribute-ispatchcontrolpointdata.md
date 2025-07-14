

- Metal
- MTLVertexAttribute
-  isPatchControlPointData 

Instance Property

# isPatchControlPointData

A Boolean value that indicates whether this vertex attribute represents control point data.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
var isPatchControlPointData: Bool { get }
```

## Discussion

This value is always false if the vertex function is not a post-tessellation vertex function.

## See Also

### Describing the Attribute

var name: String

The name of the attribute.

var attributeIndex: Int

The index of the attribute, as declared in Metal shader source code.

var attributeType: MTLDataType

The data type for the attribute, as declared in Metal shader source code.

var isActive: Bool

A Boolean value that indicates whether this vertex attribute is active.

var isPatchData: Bool

A Boolean value that indicates whether this vertex attribute represents patch data.

