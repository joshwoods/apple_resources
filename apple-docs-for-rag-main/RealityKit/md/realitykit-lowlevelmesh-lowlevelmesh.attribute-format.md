

- RealityKit
- LowLevelMesh
- LowLevelMesh.Attribute
-  format 

Instance Property

# format

The format of the vertex attribute.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
var format: MTLVertexFormat
```

## Discussion

When reading from a geometry modifier or surface shader, the value converts to its runtime representation using Metal’s standard rules.

For details about Metal’s standard rules, see format.

## See Also

### Describing an attribute

var offset: Int

The location of an attribute in vertex data, determined by the byte offset from the start of the vertex data.

var layoutIndex: Int

The index of the layout that contains this attribute.

var semantic: LowLevelMesh.VertexSemantic

The semantic of the vertex attribute, which describes how you want RealityKit to interpret the attribute.

