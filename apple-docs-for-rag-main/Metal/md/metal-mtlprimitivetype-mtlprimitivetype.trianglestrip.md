

- Metal
- MTLPrimitiveType
-  MTLPrimitiveType.triangleStrip 

Case

# MTLPrimitiveType.triangleStrip

For every three adjacent vertices, rasterize a triangle.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
case triangleStrip
```

## See Also

### Constants

case point

Rasterize a point at each vertex. The vertex shader must provide `[[point_size]]`, or the point size is undefined.

case line

Rasterize a line between each separate pair of vertices, resulting in a series of unconnected lines. If there are an odd number of vertices, the last vertex is ignored.

case lineStrip

Rasterize a line between each pair of adjacent vertices, resulting in a series of connected lines (also called a polyline).

case triangle

For every separate set of three vertices, rasterize a triangle. If the number of vertices is not a multiple of three, either one or two vertices is ignored.

