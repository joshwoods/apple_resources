

- ARKit
- ARPlaneGeometry
-  triangleIndices 

Instance Property

# triangleIndices

An array of indices describing the triangle mesh formed by the plane geometry’s vertex data.

iOS 11.3+iPadOS 11.3+

``` source
@nonobjc
var triangleIndices: [Int16] { get }
```

## Discussion

Each 16-bit integer value in this array represents an index into the vertices and textureCoordinates arrays. Each set of three indices identifies the vertices that form a single triangle in the mesh. You can use array as an index buffer for a triangle mesh in GPU-based rendering or to create 3D model asset files.

Each set of three indices forms a triangle, so the number of indices in the triangleIndices array is three times the triangleCount value.

## See Also

### Accessing Mesh Data

var vertices: [simd_float3]

An array of vertex positions for each point in the plane mesh.

var textureCoordinates: [vector_float2]

An array of texture coordinate values for each point in the plane mesh.

var triangleCount: Int

The number of triangles described by the triangleIndices buffer.

