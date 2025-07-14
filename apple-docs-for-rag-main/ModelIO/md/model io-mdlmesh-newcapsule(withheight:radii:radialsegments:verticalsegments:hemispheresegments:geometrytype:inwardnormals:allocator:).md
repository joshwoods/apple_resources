

- Model I/O
- MDLMesh
-  newCapsule(withHeight:radii:radialSegments:verticalSegments:hemisphereSegments:geometryType:inwardNormals:allocator:) 

Type Method

# newCapsule(withHeight:radii:radialSegments:verticalSegments:hemisphereSegments:geometryType:inwardNormals:allocator:)

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
class func newCapsule(
    withHeight height: Float,
    radii: vector_float2,
    radialSegments: Int,
    verticalSegments: Int,
    hemisphereSegments: Int,
    geometryType: MDLGeometryType,
    inwardNormals: Bool,
    allocator: (any MDLMeshBufferAllocator)?
) -> Self
```

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

class func newIcosahedron(withRadius: Float, inwardNormals: Bool, allocator: (any MDLMeshBufferAllocator)?) -> Self

Generates a mesh in the shape of a regular 20-sided polyhedron with triangular faces.

class func newIcosahedron(withRadius: Float, inwardNormals: Bool, geometryType: MDLGeometryType, allocator: (any MDLMeshBufferAllocator)?) -> Self

init(boxWithExtent: vector_float3, segments: vector_uint3, inwardNormals: Bool, geometryType: MDLGeometryType, allocator: (any MDLMeshBufferAllocator)?)

init(sphereWithExtent: vector_float3, segments: vector_uint2, inwardNormals: Bool, geometryType: MDLGeometryType, allocator: (any MDLMeshBufferAllocator)?)

init(cylinderWithExtent: vector_float3, segments: vector_uint2, inwardNormals: Bool, topCap: Bool, bottomCap: Bool, geometryType: MDLGeometryType, allocator: (any MDLMeshBufferAllocator)?)

init(coneWithExtent: vector_float3, segments: vector_uint2, inwardNormals: Bool, cap: Bool, geometryType: MDLGeometryType, allocator: (any MDLMeshBufferAllocator)?)

init(planeWithExtent: vector_float3, segments: vector_uint2, geometryType: MDLGeometryType, allocator: (any MDLMeshBufferAllocator)?)

init(icosahedronWithExtent: vector_float3, inwardNormals: Bool, geometryType: MDLGeometryType, allocator: (any MDLMeshBufferAllocator)?)

init(capsuleWithExtent: vector_float3, cylinderSegments: vector_uint2, hemisphereSegments: Int32, inwardNormals: Bool, geometryType: MDLGeometryType, allocator: (any MDLMeshBufferAllocator)?)

init(hemisphereWithExtent: vector_float3, segments: vector_uint2, inwardNormals: Bool, cap: Bool, geometryType: MDLGeometryType, allocator: (any MDLMeshBufferAllocator)?)

