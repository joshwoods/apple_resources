

- Model I/O
- MDLMesh
-  newEllipsoid(withRadii:radialSegments:verticalSegments:geometryType:inwardNormals:hemisphere:allocator:) 

Type Method

# newEllipsoid(withRadii:radialSegments:verticalSegments:geometryType:inwardNormals:hemisphere:allocator:)

Creates a mesh in the shape of an ellipsoid or sphere.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
class func newEllipsoid(
    withRadii radii: vector_float3,
    radialSegments: Int,
    verticalSegments: Int,
    geometryType: MDLGeometryType,
    inwardNormals: Bool,
    hemisphere: Bool,
    allocator: (any MDLMeshBufferAllocator)?
) -> Self
```

## Parameters 

`radii`  

A vector containing the width (x-component), height (y-component), and depth (z-component) of the bounding box of the ellipsoid to generate. If all components are equal, this method generates a sphere.

`radialSegments`  

The number of points to generate around the horizontal circumference of the ellipsoid (that is, its cross-section in the xz-plane). A larger number of points increases rendering fidelity but decreases rendering performance.

`verticalSegments`  

The number of points to generate along the height of the ellipsoid. A larger number of points increases rendering fidelity but decreases rendering performance.

`geometryType`  

The type of geometric primitive — triangles or quads — from which to construct the mesh.

`inwardNormals`  

true to generate normal vectors pointing toward the center of the ellipsoid; false to generate normal vectors pointing outward.

`hemisphere`  

true to generate only the upper half of the ellipsoid or sphere (a dome); false to generate a complete ellipsoid or sphere.

`allocator`  

An object responsible for allocating mesh vertex data. If `nil`, Model I/O uses an internal allocator object.

## Return Value

A new mesh object.

## Discussion

This method generates vertex data for an ellipsoid centered at the origin of its local coordinate system.

The `inwardNormals` parameter determines the direction of generated vertex normal vectors for the mesh. Specify true if the mesh will be viewed from inside (for example, for use in a sky effect), or false if the mesh will be viewed from outside.

The `allocator` parameter controls vertex data allocation for the mesh. For example, to use the MetalKit framework for loading vertex data into GPU buffers for rendering using Metal, pass a MTKMeshBufferAllocator object. By specifying an allocator, you can ensure that mesh data is copied a minimal number of times between being read from a file and being loaded into GPU memory for rendering.

## See Also

### Creating Parametric Meshes

class func newBox(withDimensions: vector_float3, segments: vector_uint3, geometryType: MDLGeometryType, inwardNormals: Bool, allocator: (any MDLMeshBufferAllocator)?) -> Self

Creates a mesh in the shape of a rectangular box or cube.

class func newCylinder(withHeight: Float, radii: vector_float2, radialSegments: Int, verticalSegments: Int, geometryType: MDLGeometryType, inwardNormals: Bool, allocator: (any MDLMeshBufferAllocator)?) -> Self

Generates a mesh in the shape of a right circular or elliptical cylinder.

class func newEllipticalCone(withHeight: Float, radii: vector_float2, radialSegments: Int, verticalSegments: Int, geometryType: MDLGeometryType, inwardNormals: Bool, allocator: (any MDLMeshBufferAllocator)?) -> Self

Generates a mesh in the shape of an elliptical or circular cone.

class func newPlane(withDimensions: vector_float2, segments: vector_uint2, geometryType: MDLGeometryType, allocator: (any MDLMeshBufferAllocator)?) -> Self

Generates a mesh in the shape of a rectangular plane.

class func newCapsule(withHeight: Float, radii: vector_float2, radialSegments: Int, verticalSegments: Int, hemisphereSegments: Int, geometryType: MDLGeometryType, inwardNormals: Bool, allocator: (any MDLMeshBufferAllocator)?) -> Self

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

