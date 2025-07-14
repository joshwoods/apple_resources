

- RealityKit
- Entity
-  Entity.CoordinateSpaceReference 

Enumeration

# Entity.CoordinateSpaceReference

Defines the coordinate space reference for transform conversion.

visionOS 2.0+

``` source
enum CoordinateSpaceReference
```

## Overview

Entity uses this option as a reference coordinate space during transform conversion.

Depending on the coordinate space that a caller entity is parented under, and whether there is an immersive space open, some transform conversion case can be inapplicable. Check out each case for more information.

## Topics

### Operators

static func == (Entity.CoordinateSpaceReference, Entity.CoordinateSpaceReference) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case immersiveSpace

A reference to an opened immersive space.

case scene

A reference to an entity’s parent window scene.

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

enum ForwardDirection

Defines the forward direction for an entity.

