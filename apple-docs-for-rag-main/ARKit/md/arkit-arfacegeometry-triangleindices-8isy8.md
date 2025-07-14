

- ARKit
- ARFaceGeometry
-  triangleIndices 

Instance Property

# triangleIndices

An array of indices describing the triangle mesh formed by the face geometry’s vertex data.

iOS 11.0+iPadOS 11.0+

``` source
@nonobjc
var triangleIndices: [Int16] { get }
```

## Discussion

Each 16-bit integer value in this array represents an index into the vertices and textureCoordinates buffers. Each set of three indices identifies the vertices that form a single triangle in the mesh. (That is, this array is appropriate for use as an index buffer for a triangle mesh in GPU-based rendering or creating 3D model asset files.)

Each set of three indices forms a triangle, so the number of indices in the triangleIndices buffer is three times the triangleCount value.

Face mesh topology is constant across ARFaceGeometry instances, so this array always describes the same arrangement of vertices. Only the vertices array changes between face meshes provided by an AR session, indicating the change in vertex positions as ARKit adapts the mesh to the shape and expression of the user’s face.

## See Also

### Accessing Mesh Data

var vertices: [simd_float3]

An array of vertex positions for each point in the face mesh.

var textureCoordinates: [vector_float2]

An array of texture coordinate values for each point in the face mesh.

var triangleCount: Int

The number of triangles described by the triangleIndices buffer.

