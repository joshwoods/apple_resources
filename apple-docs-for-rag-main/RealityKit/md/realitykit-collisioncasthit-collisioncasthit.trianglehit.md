

- RealityKit
- CollisionCastHit
-  CollisionCastHit.TriangleHit 

Structure

# CollisionCastHit.TriangleHit

Information returned when ray intersects a triangle mesh.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
struct TriangleHit
```

## Topics

### Operators

static func == (CollisionCastHit.TriangleHit, CollisionCastHit.TriangleHit) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

var faceIndex: Int

The face index for the mesh face that that the ray hit.

var uv: SIMD2&lt;Float>

The barycentric uv coordinate for where in the triangle the ray hit.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable

## See Also

### Ray casting

struct CollisionCastHit

A hit result of a collision cast.

enum CollisionCastQueryType

The kinds of ray and convex shape cast queries that you can make.

struct PixelCastHit

