

- Model I/O
- MDLGeometryType
-  MDLGeometryType.triangles 

Case

# MDLGeometryType.triangles

Each set of three consecutive indices in the submesh refers to three vertices to be rendered as a triangle.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
case triangles
```

## See Also

### Constants

case points

Each index in the submesh refers to a vertex to be rendered as a single point.

case lines

Each pair of consecutive indices in the submesh refers to two vertices to be rendered as a line segment.

case triangleStrips

The first three consecutive indices in the submesh refer to three vertices to be rendered as a triangle. Each subsequent index refers to another vertex that completes a triangle formed by connecting it to the previous two vertices.

case quads

Each set of four consecutive indices in the submesh refers to four vertices to be rendered as a quadrilateral.

case variableTopology

The submesh’s index buffer does not contain a uniform set of primitives.

