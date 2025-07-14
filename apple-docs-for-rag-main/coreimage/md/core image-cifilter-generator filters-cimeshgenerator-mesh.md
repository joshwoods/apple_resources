

- Core Image
- CIFilter
- Generator Filters
- CIMeshGenerator
-  mesh 

Instance Property

# mesh

An array that describes the mesh to render.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
var mesh: [Any] { get set }
```

**Required**

## Discussion

Specify the mesh as an array of line segments. Each line segment is stored as a CIVector instance that describes the line as a start point and an end point.

