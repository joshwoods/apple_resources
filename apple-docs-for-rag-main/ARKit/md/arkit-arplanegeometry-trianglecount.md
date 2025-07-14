

- ARKit
- ARPlaneGeometry
-  triangleCount 

Instance Property

# triangleCount

The number of triangles described by the triangleIndices buffer.

iOS 11.3+iPadOS 11.3+Mac Catalyst 13.1+

``` source
var triangleCount: Int { get }
```

## Discussion

Each set of three indices forms a triangle, so the number of indices in the triangleIndices buffer is three times the triangleCount value.

## See Also

### Accessing Mesh Data

var vertices: [simd_float3]

An array of vertex positions for each point in the plane mesh.

var textureCoordinates: [vector_float2]

An array of texture coordinate values for each point in the plane mesh.

var triangleIndices: [Int16]

An array of indices describing the triangle mesh formed by the plane geometry’s vertex data.

