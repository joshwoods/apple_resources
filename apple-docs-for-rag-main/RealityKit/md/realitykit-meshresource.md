

- RealityKit
-  MeshResource 

Class

# MeshResource

A high-level representation of a collection of vertices and edges that define a shape.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
class MeshResource
```

## Mentioned in 

Adding procedural assets to a scene

Creating a plane with low-level mesh

Reducing CPU Utilization in Your RealityKit App

## Topics

### Creating a mesh resource

static func generate(from: MeshResource.Contents) throws -> MeshResource

Create a mesh resource from contents.

static func generate(from: [MeshDescriptor]) throws -> MeshResource

Create a mesh resource from a list of mesh descriptors.

convenience init(from: [MeshDescriptor]) async throws

Initialize a mesh resource from descriptors asynchronously.

convenience init(from: MeshResource.Contents) async throws

Initialize a mesh resource from contents asynchronously.

convenience init(shape: ShapeResource) async

Generates a MeshResource from a ShapeResource.

convenience init(shape: ShapeResource)

Generates a MeshResource from a ShapeResource.

static func generateAsync(from: MeshResource.Contents) -> LoadRequest&lt;MeshResource>

Create a mesh resource from contents asynchronously.

Deprecated

static func generateAsync(from: [MeshDescriptor]) -> LoadRequest&lt;MeshResource>

Create a mesh resource from a list of mesh descriptors asynchronously.

Deprecated

### Creating a low level resource

convenience init(from: LowLevelMesh) async throws

Asynchronously creates a mesh resource from a low-level mesh.

convenience init(from: LowLevelMesh) throws

Synchronously creates a mesh resource from a low-level mesh.

var lowLevelMesh: LowLevelMesh?

The low-level mesh that this mesh is built from, if any.

### Configuring the resource

var expectedMaterialCount: Int

The number of material entries required to render the mesh resource.

func replace(with: MeshResource.Contents) throws

Replace the contents of this mesh resource.

func replace(with: MeshResource.Contents) async throws

Replace the contents of this mesh resource asynchronously.

func replaceAsync(with: MeshResource.Contents) -> LoadRequest&lt;MeshResource>

Replace the contents of this mesh resource asynchronously.

Deprecated

### Accessing resource data

var contents: MeshResource.Contents

Get the contents of the mesh asset.

### Getting a bounding box

var bounds: BoundingBox

A box that bounds the mesh.

### Creating a box

static func generateBox(size: Float, cornerRadius: Float) -> MeshResource

Creates a box mesh from a length for the box’s width, height, and depth, and a radius for the corners.

static func generateBox(size: SIMD3&lt;Float>, cornerRadius: Float) -> MeshResource

Creates a box mesh from a vector of three scalar values that represent width, height, and depth, respectively, and a radius for the corners.

static func generateBox(width: Float, height: Float, depth: Float, cornerRadius: Float, splitFaces: Bool) -> MeshResource

Creates a box mesh from a width, height, depth, a radius for the corners, and a Boolean option that splits faces.

static func generateBox(size: SIMD3&lt;Float>, majorCornerRadius: Float, minorCornerRadius: Float) -> MeshResource

Creates a box mesh from a vector of three scalar values that represent width, height, and depth, respectively, and radii for the corners.

### Creating a plane

static func generatePlane(width: Float, height: Float, cornerRadius: Float) -> MeshResource

Creates a new rectangle mesh with the specified dimensions in the entity’s xy-plane.

static func generatePlane(width: Float, depth: Float, cornerRadius: Float) -> MeshResource

Creates a new rectangle mesh with the specified dimensions in the entity’s xz-plane.

### Creating a primitive shape

static func generateSphere(radius: Float) -> MeshResource

Creates a new sphere mesh with the specified radius.

static func generateCone(height: Float, radius: Float) -> MeshResource

Creates a new cone mesh with the specified dimensions.

static func generateCylinder(height: Float, radius: Float) -> MeshResource

Creates a new cylinder mesh with the specified dimensions.

### Creating a text mesh resource

static func generateText(String, extrusionDepth: Float, font: MeshResource.Font, containerFrame: CGRect, alignment: CTTextAlignment, lineBreakMode: CTLineBreakMode) -> MeshResource

Generates a 3D mesh for rendering static text.

static func generateText(String, extrusionDepth: Float, font: MeshResource.Font, containerFrame: CGRect, alignment: CTTextAlignment, lineBreakMode: CTLineBreakMode) -> MeshResource

Generates a 3D mesh for rendering static text.

convenience init(extruding: AttributedString, textOptions: MeshResource.GenerateTextOptions, extrusionOptions: MeshResource.ShapeExtrusionOptions) async throws

Asynchronously generates a 3D mesh from a string, with options for text layout and custom extrusions.

convenience init(extruding: AttributedString, textOptions: MeshResource.GenerateTextOptions, extrusionOptions: MeshResource.ShapeExtrusionOptions) throws

Synchronously generates a 3D mesh from a string, with options for text layout and custom extrusions.

### Creating a 3D mesh by extruding a 2D path

convenience init(extruding: Path, extrusionOptions: MeshResource.ShapeExtrusionOptions) async throws

Asynchronously generates a 3D mesh by extruding a 2D path.

convenience init(extruding: Path, extrusionOptions: MeshResource.ShapeExtrusionOptions) throws

Synchronously generates a 3D mesh by extruding a 2D path.

### Creating a mesh from an anchor

convenience init(from: PlaneAnchor) async throws

convenience init(from: MeshAnchor) async throws

Creates a MeshResource from the provided MeshAnchor.

### Structures

struct Contents

Value of the contents of the resource.

struct GenerateTextOptions

A type that determines the configuration for rendering text in 2D, before it is extruded.

struct Instance

An object that transforms a model to a location.

struct JointInfluences

A buffer of vertex-joint influences which bind the mesh part’s vertices to a skeleton via a skinning deformation.

struct Model

A model consists of a list of parts.

struct Part

A part of a model consisting of a single material.

struct ShapeExtrusionOptions

A type that determines the extrusion, chamfering, and material assignment of an extruded shape.

struct Skeleton

A skeleton consists of a hierarchy of joints. Each joint defines a coordinate space. Portions of a model may be thought of as having a position in a joint’s local space.

### Type Aliases

typealias Font

A platform-specific type that represents a font for use in generating a text mesh.

## Relationships

### Conforms To

- Resource
- Sendable

## See Also

### Model display

struct ModelComponent

A component that contains a mesh and materials for the visual appearance of an entity.

class ModelEntity

A representation of a physical object that RealityKit renders and optionally simulates.

