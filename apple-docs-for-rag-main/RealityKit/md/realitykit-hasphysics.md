

- RealityKit
-  HasPhysics 

Protocol

# HasPhysics

An interface that combines the physics body and physics motion interfaces.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
protocol HasPhysics : HasPhysicsBody, HasPhysicsMotion
```

## Relationships

### Inherits From

- HasCollision
- HasPhysicsBody
- HasPhysicsMotion
- HasTransform

### Conforming Types

- ModelEntity

## See Also

### Entity compliance

protocol HasPhysicsBody

An interface that enables physics simulations based on the rules of Newtonian mechanics.

protocol HasPhysicsMotion

An interface that provides velocity properties for physics simulations.

