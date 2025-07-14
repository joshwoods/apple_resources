

- RealityKit
-  ForceEffectProtocol 

Protocol

# ForceEffectProtocol

A protocol that defines a custom force effect.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
protocol ForceEffectProtocol
```

## Overview

A custom force effect is a function of a set of input rigid body attributes and returns force-like vector quantities. You can declare this custom force effect’s input types (parameterTypes) and output types (forceMode) by conforming to `ForceEffectProtocol`.

For example, you can declare a custom force effect that depends on rigid bodies’ position and mass, and computes acceleration for each rigid body.

```
struct MyCustomForce : ForceEffectProtocol {
    var parameterTypes: PhysicsBodyParameterTypes { [.position, .mass] }
    var forceMode: ForceMode = .acceleration
    func update(parameters: inout ForceEffectParameters) {
    }
}
```

Register your custom force effect to enable the physics system to compute forces affected by rigid bodies.

```
MyCustomForce.register()
```

At each physics update, the update(parameters:) method receives the declared inputs from ForceEffectParameters. You can set the output forces for each rigid body with setForce(_:index:).

Sometimes, you may need to access properties from both your custom force effect and the current context while computing forces in the update function. The register(_:) method accepts an optional closure that allows you to capture the necessary properties. If you provide this closure to the register method, the update method is not required.

```
struct MyCustomForceClosure: ForceEffectProtocol {
    var forceMode: RealityFoundation.ForceMode = .force
    var parameterTypes: PhysicsBodyParameterTypes { [.position, .mass] }
    let customProperty: Double = 1
}

let contextualProperty: Double = 1

MyCustomForceClosure.register { event in
    // Access the effect property via `event.effect.customProperty`.
    // Access the input rigid body attributes via `event.parameters`.
    // Access the contextual property directly by `contextualProperty`.
}
```

## Topics

### Updating effects

func update(parameters: inout ForceEffectParameters)

Defines how the custom force effect computes forces at each physics simulation step.

**Required** Default implementation provided.

static func register(((inout ForceEffectEvent&lt;Self>) -> Void)?)

Registers the custom effect.

struct PhysicsBodyParameterTypes

Defines which rigid body inputs are required by a force effect’s update handler.

struct ForceEffectParameters

The force effect input data to the effect’s update handler or closure.

struct ForceEffectEvent

A struct that defines the arguments to the custom force effect update closure.

struct UnsafeForceEffectBuffer

Provides access to physics body parameters from the effect’s update function or event handler.

### Instance Properties

var forceMode: ForceMode

The mode that controls how the physics system interprets the outputs from a user’s custom force computation.

**Required**

var parameterTypes: PhysicsBodyParameterTypes

The input types to user’s custom force computation.

**Required** Default implementation provided.

### Type Methods

static func register(((inout ForceEffectEvent&lt;Self>) -> Void)?)

Register the codable custom effect. If a handler is specified, the closure is used to update the effect.

## Relationships

### Conforming Types

- ConstantForceEffect
- ConstantRadialForceEffect
- DragForceEffect
- RadialForceEffect
- TurbulenceForceEffect
- VortexForceEffect

## See Also

### Custom forces

enum ForceMode

The options that control how physics system applies the forces.

struct ForceEffectParameters

The force effect input data to the effect’s update handler or closure.

protocol ForceEffectBase

The base protocol for the wrapping force effect structure containing common parameters for all force-effects.

