

- RealityKit
- PhysicsSimulationComponent
-  PhysicsSimulationComponent.CollisionOptions 

Structure

# PhysicsSimulationComponent.CollisionOptions

The options set that defines how a physics simulation reports collisions.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
struct CollisionOptions
```

## Topics

### Initializers

init(rawValue: UInt8)

Creates a new option set from the given raw value.

### Instance Properties

let rawValue: UInt8

The corresponding value of the raw type.

### Type Aliases

typealias ArrayLiteralElement

The type of the elements of an array literal.

typealias Element

The element type of the option set.

typealias RawValue

The raw type that can be used to represent all values of the conforming type.

### Type Properties

static let all: PhysicsSimulationComponent.CollisionOptions

Reports collisions between kinematic objects and both static and kinematic objects.

static let none: PhysicsSimulationComponent.CollisionOptions

Opts out of reporting collisions.

static let reportKinematicVsKinematic: PhysicsSimulationComponent.CollisionOptions

Reports collisions between kinematic objects.

static let reportKinematicVsStatic: PhysicsSimulationComponent.CollisionOptions

Reports collisions between kinematic objects and static objects.

### Default Implementations

Equatable Implementations

OptionSet Implementations

SetAlgebra Implementations

## Relationships

### Conforms To

- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- SetAlgebra

