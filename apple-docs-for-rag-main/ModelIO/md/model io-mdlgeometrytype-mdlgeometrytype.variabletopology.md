

- Model I/O
- MDLGeometryType
-  MDLGeometryType.variableTopology 

Case

# MDLGeometryType.variableTopology

The submesh’s index buffer does not contain a uniform set of primitives.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
case variableTopology
```

## Discussion

If a submesh has non-uniform topology, its topology property contains an object describing how the arrangement of values in the index buffer combine to produce the submesh’s shape.

## See Also

### Constants

case points

Each index in the submesh refers to a vertex to be rendered as a single point.

case lines

Each pair of consecutive indices in the submesh refers to two vertices to be rendered as a line segment.

case triangles

Each set of three consecutive indices in the submesh refers to three vertices to be rendered as a triangle.

case triangleStrips

The first three consecutive indices in the submesh refer to three vertices to be rendered as a triangle. Each subsequent index refers to another vertex that completes a triangle formed by connecting it to the previous two vertices.

case quads

Each set of four consecutive indices in the submesh refers to four vertices to be rendered as a quadrilateral.

