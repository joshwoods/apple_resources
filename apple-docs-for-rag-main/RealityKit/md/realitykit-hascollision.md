

- RealityKit
-  HasCollision 

Protocol

# HasCollision

An interface used for ray casting and collision detection.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
protocol HasCollision : HasTransform
```

## Topics

### Getting the component

var collision: CollisionComponent?

The collision component that gives the entity the ability to participate in collision simulations.

## Relationships

### Inherits From

- HasTransform

### Inherited By

- HasPhysics
- HasPhysicsBody

### Conforming Types

- ModelEntity
- TriggerVolume

