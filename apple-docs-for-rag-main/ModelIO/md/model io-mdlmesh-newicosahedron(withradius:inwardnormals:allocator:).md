

- Model I/O
- MDLMesh
-  newIcosahedron(withRadius:inwardNormals:allocator:) 

Type Method

# newIcosahedron(withRadius:inwardNormals:allocator:)

Generates a mesh in the shape of a regular 20-sided polyhedron with triangular faces.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
class func newIcosahedron(
    withRadius radius: Float,
    inwardNormals: Bool,
    allocator: (any MDLMeshBufferAllocator)?
) -> Self
```

## Parameters 

`radius`  

The distance from the icosahedron’s center to any one of its vertices.

`inwardNormals`  

true to generate normal vectors pointing toward the center of the icosahedron; false to generate normal vectors pointing outward.

`allocator`  

An object responsible for allocating mesh vertex data. If `nil`, Model I/O uses an internal allocator object.

## Return Value

A new mesh object.

## Discussion

This method generates vertex data for an icosahedron centered at the origin of its local coordinate system. An icosahedron is a rough approximation of a sphere—to generate a more precise approximation, create an icosahedron and use the newSubdividedMesh(_:submeshIndex:subdivisionLevels:) method to turn it into a geodesic sphere.

The `inwardNormals` parameter determines the direction of generated vertex normal vectors for the mesh. Specify true if the mesh will be viewed from inside (for example, for use in a sky effect), or false if the mesh will be viewed from outside.

## See Also

### Creating Parametric Meshes

class func newBox(withDimensions: vector_float3, segments: vector_uint3, geometryType: MDLGeometryType, inwardNormals: Bool, allocator: (any MDLMeshBufferAllocator)?) -> Self

Creates a mesh in the shape of a rectangular box or cube.

class func newEllipsoid(withRadii: vector_float3, radialSegments: Int, verticalSegments: Int, geometryType: MDLGeometryType, inwardNormals: Bool, hemisphere: Bool, allocator: (any MDLMeshBufferAllocator)?) -> Self

Creates a mesh in the shape of an ellipsoid or sphere.

class func newCylinder(withHeight: Float, radii: vector_float2, radialSegments: Int, verticalSegments: Int, geometryType: MDLGeometryType, inwardNormals: Bool, allocator: (any MDLMeshBufferAllocator)?) -> Self

Generates a mesh in the shape of a right circular or elliptical cylinder.

class func newEllipticalCone(withHeight: Float, radii: vector_float2, radialSegments: Int, verticalSegments: Int, geometryType: MDLGeometryType, inwardNormals: Bool, allocator: (any MDLMeshBufferAllocator)?) -> Self

Generates a mesh in the shape of an elliptical or circular cone.

class func newPlane(withDimensions: vector_float2, segments: vector_uint2, geometryType: MDLGeometryType, allocator: (any MDLMeshBufferAllocator)?) -> Self

Generates a mesh in the shape of a rectangular plane.

class func newCapsule(withHeight: Float, radii: vector_float2, radialSegments: Int, verticalSegments: Int, hemisphereSegments: Int, geometryType: MDLGeometryType, inwardNormals: Bool, allocator: (any MDLMeshBufferAllocator)?) -> Self

class func newIcosahedron(withRadius: Float, inwardNormals: Bool, geometryType: MDLGeometryType, allocator: (any MDLMeshBufferAllocator)?) -> Self

init(boxWithExtent: vector_float3, segments: vector_uint3, inwardNormals: Bool, geometryType: MDLGeometryType, allocator: (any MDLMeshBufferAllocator)?)

init(sphereWithExtent: vector_float3, segments: vector_uint2, inwardNormals: Bool, geometryType: MDLGeometryType, allocator: (any MDLMeshBufferAllocator)?)

init(cylinderWithExtent: vector_float3, segments: vector_uint2, inwardNormals: Bool, topCap: Bool, bottomCap: Bool, geometryType: MDLGeometryType, allocator: (any MDLMeshBufferAllocator)?)

init(coneWithExtent: vector_float3, segments: vector_uint2, inwardNormals: Bool, cap: Bool, geometryType: MDLGeometryType, allocator: (any MDLMeshBufferAllocator)?)

init(planeWithExtent: vector_float3, segments: vector_uint2, geometryType: MDLGeometryType, allocator: (any MDLMeshBufferAllocator)?)

init(icosahedronWithExtent: vector_float3, inwardNormals: Bool, geometryType: MDLGeometryType, allocator: (any MDLMeshBufferAllocator)?)

init(capsuleWithExtent: vector_float3, cylinderSegments: vector_uint2, hemisphereSegments: Int32, inwardNormals: Bool, geometryType: MDLGeometryType, allocator: (any MDLMeshBufferAllocator)?)

init(hemisphereWithExtent: vector_float3, segments: vector_uint2, inwardNormals: Bool, cap: Bool, geometryType: MDLGeometryType, allocator: (any MDLMeshBufferAllocator)?)

