

- RealityKit
-  Transform 

Structure

# Transform

A component that defines the scale, rotation, and translation of an entity.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@frozen
struct Transform
```

## Overview

An entity acquires a Transform component, as well as a set of methods for manipulating the transform, by adopting the HasTransform protocol. This is true for all entities, because the Entity base class adopts the protocol.

## Topics

### Creating a transform

init()

Creates a transform with the values of the identity transform.

init(scale: SIMD3&lt;Float>, rotation: simd_quatf, translation: SIMD3&lt;Float>)

Creates a new transformation using the given values.

init(pitch: Float, yaw: Float, roll: Float)

Creates a new transform from the specified Euler angles.

init(matrix: float4x4)

Creates a new transform represented as a 4x4 matrix.

### Setting transform properties

var scale: SIMD3&lt;Float>

The scaling factor applied to the entity.

var rotation: simd_quatf

The rotation of the entity specified as a unit quaternion.

var translation: SIMD3&lt;Float>

The position of the entity along the x, y, and z axes.

var matrix: float4x4

The transform represented as a 4x4 matrix.

### Getting the identity transform

static let identity: Transform

The identity transform.

### Comparing transforms

static func == (Transform, Transform) -> Bool

Returns a Boolean value indicating whether two values are equal.

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

func hash(into: inout Hasher)

Hashes the essential components of the transform by feeding them into the given hash function.

var hashValue: Int

The hash value.

### Registering a component type

static func registerComponent()

Registers a new component type.

### Initializers

init(AffineTransform3D)

### Default Implementations

Component Implementations

Decodable Implementations

Encodable Implementations

Equatable Implementations

## Relationships

### Conforms To

- AnimatableData
- BindableData
- BitwiseCopyable
- Component
- Copyable
- Decodable
- Encodable
- Equatable
- Hashable
- Sendable

## See Also

### Positioning entities in space

protocol HasTransform

An interface that enables manipulating the scale, rotation, and translation of an entity.

func transformMatrix(relativeTo: Entity.CoordinateSpaceReference) -> float4x4?

Returns the 4 x 4 transform matrix of an entity relative to the given coordinate space.

enum CoordinateSpaceReference

Defines the coordinate space reference for transform conversion.

enum ForwardDirection

Defines the forward direction for an entity.

