

- RealityKit
-  PhysicsMaterialResource 

Class

# PhysicsMaterialResource

Material properties, like friction, of a physically simulated object.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
class PhysicsMaterialResource
```

## Topics

### Using the default material resource

static let `default`: PhysicsMaterialResource

A default material resource.

### Creating a custom material resource

static func generate(friction: Float, restitution: Float) -> PhysicsMaterialResource

Generates a new material with the given characteristics.

static func generate(staticFriction: Float, dynamicFriction: Float, restitution: Float) -> PhysicsMaterialResource

Creates a new material with the specified static friction, dynamic friction, and restitution.

## Relationships

### Conforms To

- Resource
- Sendable

## See Also

### Physical properties

struct PhysicsBodyComponent

A component that defines an entity’s behavior in physics body simulations.

enum PhysicsBodyMode

The ways that a physics body can move in response to physical forces.

struct PhysicsMassProperties

Mass properties of a physics body.

