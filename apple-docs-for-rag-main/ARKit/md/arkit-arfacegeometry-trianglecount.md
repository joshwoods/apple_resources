

- ARKit
- ARFaceGeometry
-  triangleCount 

Instance Property

# triangleCount

The number of triangles described by the triangleIndices buffer.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
var triangleCount: Int { get }
```

## Discussion

Each set of three indices forms a triangle, so the number of indices in the triangleIndices buffer is three times the triangleCount value.

Face mesh topology is constant across ARFaceGeometry instances, so the value of this property is the same for all instances.

## See Also

### Accessing Mesh Data

var vertices: [simd_float3]

An array of vertex positions for each point in the face mesh.

var textureCoordinates: [vector_float2]

An array of texture coordinate values for each point in the face mesh.

var triangleIndices: [Int16]

An array of indices describing the triangle mesh formed by the face geometry’s vertex data.

