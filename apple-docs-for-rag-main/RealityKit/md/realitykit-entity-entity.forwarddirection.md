

- RealityKit
- Entity
-  Entity.ForwardDirection 

Enumeration

# Entity.ForwardDirection

Defines the forward direction for an entity.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
enum ForwardDirection
```

## Topics

### Operators

static func == (Entity.ForwardDirection, Entity.ForwardDirection) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case negativeZ

case positiveZ

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable

## See Also

### Positioning entities in space

protocol HasTransform

An interface that enables manipulating the scale, rotation, and translation of an entity.

struct Transform

A component that defines the scale, rotation, and translation of an entity.

func transformMatrix(relativeTo: Entity.CoordinateSpaceReference) -> float4x4?

Returns the 4 x 4 transform matrix of an entity relative to the given coordinate space.

enum CoordinateSpaceReference

Defines the coordinate space reference for transform conversion.

