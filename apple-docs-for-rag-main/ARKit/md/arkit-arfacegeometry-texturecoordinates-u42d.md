

- ARKit
- ARFaceGeometry
-  textureCoordinates 

Instance Property

# textureCoordinates

An array of texture coordinate values for each point in the face mesh.

iOS 11.0+iPadOS 11.0+

``` source
@nonobjc
var textureCoordinates: [vector_float2] { get }
```

## Discussion

Each `float2` value in this array represents the UV texture coordinates for the vertex at the corresponding index in the vertices buffer.Face mesh topology is constant across ARFaceGeometry instances, so the values in this array always maps the same vertex indices to the same texture coordinates.

## See Also

### Accessing Mesh Data

var vertices: [simd_float3]

An array of vertex positions for each point in the face mesh.

var triangleCount: Int

The number of triangles described by the triangleIndices buffer.

var triangleIndices: [Int16]

An array of indices describing the triangle mesh formed by the face geometry’s vertex data.

