

- ARKit
- ARPlaneGeometry
-  textureCoordinates 

Instance Property

# textureCoordinates

An array of texture coordinate values for each point in the plane mesh.

iOS 11.3+iPadOS 11.3+

``` source
@nonobjc
var textureCoordinates: [vector_float2] { get }
```

## Discussion

Each `float2` value in this array represents the UV texture coordinates for the vertex at the corresponding index in the vertices array.

## See Also

### Accessing Mesh Data

var vertices: [simd_float3]

An array of vertex positions for each point in the plane mesh.

var triangleCount: Int

The number of triangles described by the triangleIndices buffer.

var triangleIndices: [Int16]

An array of indices describing the triangle mesh formed by the plane geometry’s vertex data.

