

- RealityKit
-  OrientedBoundingBox 

Structure

# OrientedBoundingBox

Representation for an oriented bounding box. Uses a combination of an axis-aligned bounding box and a rotation vector around the centroid of the said axis-aligned bounding box to represent an oriented bounding box.

iOS 17.0+iPadOS 17.0+Mac Catalyst 16.0+macOS 13.0+

``` source
struct OrientedBoundingBox
```

## Topics

### Operators

static func == (OrientedBoundingBox, OrientedBoundingBox) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Initializers

init(orientation: simd_quatf, boundingBox: BoundingBox)

### Instance Properties

var boundingBox: BoundingBox

Axis aligned bounding box

var hashValue: Int

The hash value.

var orientation: simd_quatf

Orientation (rotation) of the bounding box

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable
- Hashable

## See Also

### Bounding box retrieval

struct BoundingBox

An axis-aligned bounding box (AABB).

