

- RealityKit
-  ShapeResource 

Class

# ShapeResource

A representation of a shape.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
class ShapeResource
```

## Topics

### Transforming a shape

func offsetBy(rotation: simd_quatf) -> ShapeResource

Creates a new shape resource by applying a rotation.

func offsetBy(translation: SIMD3&lt;Float>) -> ShapeResource

Creates a new shape resource by applying a translation.

func offsetBy(rotation: simd_quatf, translation: SIMD3&lt;Float>) -> ShapeResource

Creates a new shape resource by applying a rotation and a translation.

### Generating boxes

static func generateBox(size: SIMD3&lt;Float>) -> ShapeResource

Creates a box shape with the specified extent.

static func generateBox(width: Float, height: Float, depth: Float) -> ShapeResource

Creates a box shape with the specified dimensions.

### Generating spheres

static func generateSphere(radius: Float) -> ShapeResource

Creates a sphere shape with the specified radius.

### Generating capsules

static func generateCapsule(height: Float, radius: Float) -> ShapeResource

Creates a capsule shape with the specified height and radius.

### Generating convex shapes

static func generateConvex(from: [SIMD3&lt;Float>]) -> ShapeResource

Creates a convex shape from the given points.

static func generateConvex(from: MeshResource) -> ShapeResource

Creates a convex shape from the given mesh.

### Comparing shapes

static func == (ShapeResource, ShapeResource) -> Bool

Indicates whether two shapes are equal.

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

func hash(into: inout Hasher)

Hashes the essential components of the shape by feeding them into the given hash function.

var hashValue: Int

The hash value.

### Instance Properties

var bounds: BoundingBox

Axis aligned bounding box in world space.

### Type Methods

static func generateConvex(from: [SIMD3&lt;Float>]) async throws -> ShapeResource

Creates a convex shape from the given points asynchronously.

static func generateConvex(from: MeshResource) async throws -> ShapeResource

Creates a convex shape from the given mesh.

static func generateStaticMesh(from: MeshAnchor) async throws -> ShapeResource

Creates a mesh-based collision shape derived from an ARKit scene-understanding mesh anchor.

static func generateStaticMesh(from: MeshResource) async throws -> ShapeResource

Creates a static collision mesh from a mesh resource.

static func generateStaticMesh(from: ARMeshAnchor) async throws -> ShapeResource

static func generateStaticMesh(positions: [SIMD3&lt;Float>], faceIndices: [UInt16]) async throws -> ShapeResource

Creates a static collision mesh from an array of vertex positions and face indices.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable
- Hashable
- Resource
- Sendable

## See Also

### Collision shapes and groups

Simulating physics with collisions in your visionOS app

Create entities that behave and react like physical objects in a RealityKit view.

Configuring Collision in RealityKit

Use collision groups and collision filters to control which objects collide.

struct CollisionComponent

A component that gives an entity the ability to collide with other entities that also have collision components.

enum Mode

A mode that dictates how much collision data is collected for a given entity.

enum ShapeResourceError

struct CollisionGroup

A bitmask used to define the collision group to which an entity belongs.

struct CollisionFilter

A set of masks that determine whether entities can collide during simulations.

class TriggerVolume

An invisible 3D shape that detects when objects enter or exit a given region of space.

