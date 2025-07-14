

- RealityKit
-  PixelCastHit 

Structure

# PixelCastHit

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+

``` source
struct PixelCastHit
```

## Topics

### Operators

static func == (PixelCastHit, PixelCastHit) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

var barycentric: SIMD3&lt;Float>?

The barycentric coordinate of the primitive. See the discussion of \[\[barycentric_coord\]\] in Section “5.2.3.4 Fragment Function Input Attributes” of Metal Shading Language Specification

var entity: Entity

The entity that was hit.

var instance: UInt32

The instance within the MeshResource of the intersection. This can be used to index into MeshResource.contents.instances

var meshPart: UInt64

The mesh part id of the entity that was selected by the hit.

var normal: SIMD3&lt;Float>

The surface normal at the point of intersection, in scene space.

var position: SIMD3&lt;Float>

The surface position at the point of intersection, in scene space.

var primitive: UInt32

The per-primitive identifier used with barycentric coordinates.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable
- Sendable

## See Also

### Entity searches

struct QueryPredicate

An object that defines the criteria for an entity query.

