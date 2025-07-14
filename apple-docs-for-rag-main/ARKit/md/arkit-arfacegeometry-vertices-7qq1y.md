

- ARKit
- ARFaceGeometry
-  vertices 

Instance Property

# vertices

An array of vertex positions for each point in the face mesh.

iOS 11.0+iPadOS 11.0+

``` source
@nonobjc
var vertices: [simd_float3] { get }
```

## Discussion

Each `float3` value in this array represents the position of a vertex in the mesh, in face coordinates. (See Tracking Face Position and Orientation.)

## See Also

### Accessing Mesh Data

var textureCoordinates: [vector_float2]

An array of texture coordinate values for each point in the face mesh.

var triangleCount: Int

The number of triangles described by the triangleIndices buffer.

var triangleIndices: [Int16]

An array of indices describing the triangle mesh formed by the face geometry’s vertex data.

