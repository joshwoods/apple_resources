

- RealityKit
- LowLevelMesh
- LowLevelMesh.Attribute
-  layoutIndex 

Instance Property

# layoutIndex

The index of the layout that contains this attribute.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
var layoutIndex: Int
```

## Discussion

The index refers to an entry in vertexLayouts.

## See Also

### Describing an attribute

var format: MTLVertexFormat

The format of the vertex attribute.

var offset: Int

The location of an attribute in vertex data, determined by the byte offset from the start of the vertex data.

var semantic: LowLevelMesh.VertexSemantic

The semantic of the vertex attribute, which describes how you want RealityKit to interpret the attribute.

