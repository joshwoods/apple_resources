

- RealityKit
- LowLevelMesh
- LowLevelMesh.Attribute
-  semantic 

Instance Property

# semantic

The semantic of the vertex attribute, which describes how you want RealityKit to interpret the attribute.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
var semantic: LowLevelMesh.VertexSemantic
```

## Discussion

RealityKit consults the vertex semantic when interpreting the data in your LowLevelMesh. For example, an attribute with the semantic value of LowLevelMesh.VertexSemantic.position uses to determine the position of a vertex.

## See Also

### Describing an attribute

var format: MTLVertexFormat

The format of the vertex attribute.

var offset: Int

The location of an attribute in vertex data, determined by the byte offset from the start of the vertex data.

var layoutIndex: Int

The index of the layout that contains this attribute.

