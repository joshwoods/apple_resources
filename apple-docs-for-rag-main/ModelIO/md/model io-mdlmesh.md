

- Model I/O
-  MDLMesh 

Class

# MDLMesh

A container for vertex buffer data to be used in rendering a 3D object.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
class MDLMesh
```

## Overview

A mesh contains one or more MDLSubmesh objects. Each submesh contains index buffer data that describes how the mesh’s vertices should be combined for drawing and references material information describing an intended surface appearance for the submesh. Typically, you obtain meshes by traversing the object hierarchy of a MDLAsset object, but you can also create meshes from your own vertex data or create parametric meshes. The MDLMesh class also supports processing meshes to generate vertex attributes or to bake lighting information.

## Topics

### Creating a Custom Mesh

init(vertexBuffer: any MDLMeshBuffer, vertexCount: Int, descriptor: MDLVertexDescriptor, submeshes: [MDLSubmesh])

Creates a mesh from a single vertex buffer with the specified parameters.

init(vertexBuffers: [any MDLMeshBuffer], vertexCount: Int, descriptor: MDLVertexDescriptor, submeshes: [MDLSubmesh])

Creates a mesh by unifying vertex data from multiple sources with the specified parameters.

init(bufferAllocator: (any MDLMeshBufferAllocator)?)

class func newSubdividedMesh(MDLMesh, submeshIndex: Int, subdivisionLevels: Int) -> Self?

Creates a new mesh by subdividing the specified mesh.

init(meshBySubdividingMesh: MDLMesh, submeshIndex: Int32, subdivisionLevels: UInt32, allocator: (any MDLMeshBufferAllocator)?)

### Working with Vertex Data

var boundingBox: MDLAxisAlignedBoundingBox

The minimum region entirely enclosing the mesh’s vertex positions, expressed in the model coordinate system of the mesh.

var submeshes: NSMutableArray?

The array of submeshes to be used in rendering the mesh.

var vertexBuffers: [any MDLMeshBuffer]

The array of buffers that provide vertex data for the mesh.

var vertexCount: Int

The number of vertices in the mesh.

var vertexDescriptor: MDLVertexDescriptor

A description of the format and layout of the mesh’s vertex buffers.

var allocator: any MDLMeshBufferAllocator

func addAttribute(withName: String, format: MDLVertexFormat)

Adds a vertex attribute to the mesh and creates a new, empty corresponding vertex buffer.

func addAttribute(withName: String, format: MDLVertexFormat, type: String, data: Data, stride: Int)

func addAttribute(withName: String, format: MDLVertexFormat, type: String, data: Data, stride: Int, time: TimeInterval)

func removeAttributeNamed(String)

func replaceAttributeNamed(String, with: MDLVertexAttributeData)

func updateAttributeNamed(String, with: MDLVertexAttributeData)

func addUnwrappedTextureCoordinates(forAttributeNamed: String)

func vertexAttributeData(forAttributeNamed: String) -> MDLVertexAttributeData?

Returns the vertex data for the specified attribute.

func vertexAttributeData(forAttributeNamed: String, as: MDLVertexFormat) -> MDLVertexAttributeData?

### Generating Geometry Data

func addNormals(withAttributeNamed: String?, creaseThreshold: Float)

Generates surface normal data for the mesh based on its vertex position data.

func addTangentBasis(forTextureCoordinateAttributeNamed: String, tangentAttributeNamed: String, bitangentAttributeNamed: String?)

Generates surface tangent and bitangent data for the mesh based on its vertex position and texture coordinate data.

func addTangentBasis(forTextureCoordinateAttributeNamed: String, normalAttributeNamed: String, tangentAttributeNamed: String)

Generates surface tangent data for the mesh based on its vertex position, surface normal, and texture coordinate data.

func makeVerticesUnique()

Modifies the mesh’s vertex buffers so that no vertices are shared by multiple faces.

Deprecated

### Generating Ambient Occlusion Data

func generateAmbientOcclusionTexture(withQuality: Float, attenuationFactor: Float, objectsToConsider: [MDLObject], vertexAttributeNamed: String, materialPropertyNamed: String) -> Bool

Calculates ambient occlusion (AO) information for the mesh and saves it in the mesh as a material property texture.

func generateAmbientOcclusionTexture(withSize: vector_int2, raysPerSample: Int, attenuationFactor: Float, objectsToConsider: [MDLObject], vertexAttributeNamed: String, materialPropertyNamed: String) -> Bool

Calculates ambient occlusion (AO) information for the mesh and saves it in the mesh as a material property texture of the specified size.

func generateAmbientOcclusionVertexColors(withQuality: Float, attenuationFactor: Float, objectsToConsider: [MDLObject], vertexAttributeNamed: String) -> Bool

Calculates ambient occlusion (AO) information for the mesh and saves it in the mesh as a vertex color attribute.

func generateAmbientOcclusionVertexColors(withRaysPerSample: Int, attenuationFactor: Float, objectsToConsider: [MDLObject], vertexAttributeNamed: String) -> Bool

Calculates ambient occlusion (AO) information for the mesh, using the specified number of rays per sample, and saves it in the mesh as a vertex color attribute.

### Generating Light Map Data

func generateLightMapTexture(withQuality: Float, lightsToConsider: [MDLLight], objectsToConsider: [MDLObject], vertexAttributeNamed: String, materialPropertyNamed: String) -> Bool

Calculates static lighting information for the mesh and saves it in the mesh as a material property texture.

func generateLightMapTexture(withTextureSize: vector_int2, lightsToConsider: [MDLLight], objectsToConsider: [MDLObject], vertexAttributeNamed: String, materialPropertyNamed: String) -> Bool

Calculates static lighting information for the mesh and saves it in the mesh as a material property texture of the specified size.

func generateLightMapVertexColorsWithLights(toConsider: [MDLLight], objectsToConsider: [MDLObject], vertexAttributeNamed: String) -> Bool

Calculates static lighting information for the mesh and saves it in the mesh as a vertex color attribute.

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

### Instance Methods

func addOrthTanBasis(forTextureCoordinateAttributeNamed: String, normalAttributeNamed: String, tangentAttributeNamed: String)

func flipTextureCoordinates(inAttributeNamed: String)

func makeVerticesUniqueAndReturnError() throws

## Relationships

### Inherits From

- MDLObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- MDLNamed
- NSObjectProtocol

## See Also

### 3D Asset Basics

class MDLAsset

An indexed container for 3D objects and associated information, such as transform hierarchies, meshes, cameras, and lights.

class MDLObject

The base class for objects that are part of a 3D asset, including meshes, cameras, and lights.

class MDLTransform

A description of the local coordinate space transformations for a 3D object.

class MDLSubmesh

A container for index buffer data and material information to be used in rendering all or part of a 3D object.

class MDLSubmeshTopology

A description of how a submesh’s index buffer data is arranged and how that arrangement should be used to produce the submesh’s intended 3D shape.

protocol MDLNamed

The common interface for Model I/O objects that expose a human-readable name.

