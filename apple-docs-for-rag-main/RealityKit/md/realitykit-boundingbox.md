

- RealityKit
-  BoundingBox 

Structure

# BoundingBox

An axis-aligned bounding box (AABB).

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@frozen
struct BoundingBox
```

## Topics

### Creating a bounding box

init()

Creates an empty bounding box.

init(min: SIMD3&lt;Float>, max: SIMD3&lt;Float>)

Creates a bounding box with the given settings.

### Getting an empty box

static let empty: BoundingBox

An empty bounding box.

var isEmpty: Bool

A Boolean that indicates whether the bounding box is empty.

### Getting the box characteristics

var max: SIMD3&lt;Float>

The position of the maximum corner of the box.

var min: SIMD3&lt;Float>

The position of the minimum corner of the box.

var center: SIMD3&lt;Float>

The center of the bounding box.

var extents: SIMD3&lt;Float>

The extents of the bounding box.

var boundingRadius: Float

The radius of a bounding sphere that encompasses the bounding box.

### Expanding boxes

func union(BoundingBox) -> BoundingBox

Creates a bounding box containing the current bounds and the specified bounds.

func formUnion(BoundingBox)

Expands the bounding box to contain the specified bounds.

func union(SIMD3&lt;Float>) -> BoundingBox

Creates a bounding box containing the current bounds and the specified point.

func formUnion(SIMD3&lt;Float>)

Expands the bounding box to contain the specified point.

### Checking for overlap

func contains(BoundingBox) -> Bool

Checks whether the bounding box contains the specified bounds.

func contains(SIMD3&lt;Float>) -> Bool

Checks whether the bounding box contains the specified point.

func intersects(BoundingBox) -> Bool

Checks whether the bounding box intersects the specified bounds.

### Checking for separation

func distanceSquared(toPoint: SIMD3&lt;Float>) -> Float

Calculates the distance from a point to the bounding box.

### Transforming a bounding box

func transform(by: float4x4)

Transforms the bounding box.

func transformed(by: float4x4) -> BoundingBox

Transforms the bounding box and finds the bounds of the result.

### Comparing bounding boxes

static func == (BoundingBox, BoundingBox) -> Bool

Indicates whether two bounding boxes are equal.

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

func hash(into: inout Hasher)

Hashes the essential components of the bounding box by feeding them into the given hash function.

var hashValue: Int

The hash value.

### Initializers

init(Rect3D)

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- BitwiseCopyable
- Copyable
- Equatable
- Hashable
- Sendable

## See Also

### Bounding box retrieval

struct OrientedBoundingBox

Representation for an oriented bounding box. Uses a combination of an axis-aligned bounding box and a rotation vector around the centroid of the said axis-aligned bounding box to represent an oriented bounding box.

