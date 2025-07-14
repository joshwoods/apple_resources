

- RealityKit
-  CollisionCastQueryType 

Enumeration

# CollisionCastQueryType

The kinds of ray and convex shape cast queries that you can make.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
enum CollisionCastQueryType
```

## Topics

### Collision cast queries

case nearest

Report the closest hit.

case all

Report all hits sorted in ascending order by distance from the cast origin.

case any

Report one hit.

### Comparing collision cast queries

static func == (CollisionCastQueryType, CollisionCastQueryType) -> Bool

Returns a Boolean value indicating whether two values are equal.

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

var hashValue: Int

The hash value.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable
- Hashable

## See Also

### Ray casting

struct CollisionCastHit

A hit result of a collision cast.

struct TriangleHit

Information returned when ray intersects a triangle mesh.

struct PixelCastHit

