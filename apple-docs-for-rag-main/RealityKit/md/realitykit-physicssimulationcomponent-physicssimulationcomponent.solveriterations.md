

- RealityKit
- PhysicsSimulationComponent
-  PhysicsSimulationComponent.SolverIterations 

Structure

# PhysicsSimulationComponent.SolverIterations

The parameters that control the accuracy of solving physics simulations.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
struct SolverIterations
```

## Topics

### Operators

static func == (PhysicsSimulationComponent.SolverIterations, PhysicsSimulationComponent.SolverIterations) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Initializers

init(positionIterations: Int, velocityIterations: Int)

Creates a solver iterations configuration.

### Instance Properties

var positionIterations: Int

The number of position iterations the solver performs.

var velocityIterations: Int

The number of velocity iterations the solver performs.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable

