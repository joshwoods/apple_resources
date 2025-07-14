

- RealityKit
-  ForceEffectComponent 

Structure

# ForceEffectComponent

A component that defines the forces that affect an entity, including custom forces that you define.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
struct ForceEffectComponent
```

## Overview

After you assign a `ForceEffectComponent` to an entity, the force effects in the component apply each physics update for as long as the component and force effects exist. Each ForceEffect updates sequentially while the physics system accumulates its forces. The center frame of each ForceEffect coincides with and moves alongside the entity’s position and orientation. To offset this center frame, set the position and orientation.

Note

You can set the simulationState parameter to ForceEffectComponent.SimulationState.pause if you want to apply forces later.

### Create forces

Use ConstantForceEffect to apply a constant force in a direction:

```
let constantForceEffect = ForceEffect(effect: ConstantForceEffect(strength: 1, direction: [1, 0, 0]))
```

RealityKit provides a set of useful forces you can use with `ForceEffectComponent`:

- ConstantForceEffect

- ConstantRadialForceEffect

- DragForceEffect

- RadialForceEffect

- TurbulenceForceEffect

- VortexForceEffect

### Create custom forces

To create a custom force effect, define a structure that implements ForceEffectProtocol, then create an instance of ForceEffectBase with your custom `ForceEffectProtocol` implementation:

```
// CustomForce implements ForceEffectProtocol, and has a custom parameter, thrustersActive, that determines how the system applies your force to a physics body.
let thrusterForce = CustomForce(thrustersActive: true)
// Create an instance of ForceEffectBase using your custom force.
let thursterForceEffect = ForceEffect(effect: thrusterForce)
```

Note

To apply force to a physics body with a custom `ForceEffectProtocol`, you must implement and apply forces in update(parameters:).

### Apply forces

You can apply multiple forces to your entity at once by including them in `ForceEffectComponent`:

```
let forceEffectComponent = ForceEffectComponent(effects: [constantForceEffect, thrusterForceEffect])
entity.components.set(forceEffectComponent)
```

## Topics

### Initializers

init(effect: any ForceEffectBase)

Creates a force effect component with a single force effect, and automatically plays it.

init(effects: [any ForceEffectBase], simulationState: ForceEffectComponent.SimulationState)

Creates a force effect component.

### Instance Properties

var effects: [any ForceEffectBase]

One or more effects used to simulate forces.

var simulationState: ForceEffectComponent.SimulationState?

The desired state of the simulation.

### Enumerations

enum SimulationState

The simulation runtime states.

### Default Implementations

Component Implementations

## Relationships

### Conforms To

- Component

## See Also

### Force effect components

struct ForceEffect

Defines a force effect’s system, and type specific properties.

