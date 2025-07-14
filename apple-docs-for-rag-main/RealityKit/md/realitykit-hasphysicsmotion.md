

- RealityKit
-  HasPhysicsMotion 

Protocol

# HasPhysicsMotion

An interface that provides velocity properties for physics simulations.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
protocol HasPhysicsMotion : Entity
```

## Topics

### Setting the motion component

var physicsMotion: PhysicsMotionComponent?

The physics motion component used by physics simulations of the model entity.

## Relationships

### Inherits From

- Entity

### Inherited By

- HasPhysics

### Conforming Types

- ModelEntity

## See Also

### Entity compliance

protocol HasPhysicsBody

An interface that enables physics simulations based on the rules of Newtonian mechanics.

protocol HasPhysics

An interface that combines the physics body and physics motion interfaces.

