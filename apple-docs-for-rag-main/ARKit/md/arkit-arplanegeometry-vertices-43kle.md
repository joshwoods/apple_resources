

- ARKit
- ARPlaneGeometry
-  vertices 

Instance Property

# vertices

An array of vertex positions for each point in the plane mesh.

iOS 11.3+iPadOS 11.3+

``` source
@nonobjc
var vertices: [simd_float3] { get }
```

## Discussion

Each `float3` value in this array represents the position of a vertex in the mesh. The owning plane anchor’s transform matrix defines the coordinate system for these points.

This array, together with the triangleIndices array, describes a mesh covering the entire surface of the plane. Use this mesh for purposes that involve the filled shape, such as rendering a solid 3D representation of the surface. If, instead, you only need to know the outline of the shape, see the boundaryVertices property.

## See Also

### Accessing Mesh Data

var textureCoordinates: [vector_float2]

An array of texture coordinate values for each point in the plane mesh.

var triangleCount: Int

The number of triangles described by the triangleIndices buffer.

var triangleIndices: [Int16]

An array of indices describing the triangle mesh formed by the plane geometry’s vertex data.

