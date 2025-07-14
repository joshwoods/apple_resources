

- RealityKit
- LowLevelMesh
- LowLevelMesh.Attribute
-  offset 

Instance Property

# offset

The location of an attribute in vertex data, determined by the byte offset from the start of the vertex data.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
var offset: Int
```

## See Also

### Describing an attribute

var format: MTLVertexFormat

The format of the vertex attribute.

var layoutIndex: Int

The index of the layout that contains this attribute.

var semantic: LowLevelMesh.VertexSemantic

The semantic of the vertex attribute, which describes how you want RealityKit to interpret the attribute.

