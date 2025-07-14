

- RealityKit
-  OpacityComponent 

Structure

# OpacityComponent

A component that controls the opacity of an entity and its descendants.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
struct OpacityComponent
```

## Overview

An opacity component multiplies its opacity property with all visual components the entity and its descendants own. Visual components include ModelComponent and ParticleEmitterComponent. If a descendant also has its own opacity component, the system combines the two opacities by multiplying their values. The system repeats this pattern for the entity’s entire family tree.

For example, the following code sets a component’s opacity value to `0.5` for its entity:

```
// Load a USDZ model from a file, or create a model component.
let robot = try await Entity(named: "vintage_robot")

// Create an opacity component.
let opacityComponent = OpacityComponent(opacity: 0.5)

// Apply the opacity component to the robot entity.
robot.components.set(opacityComponent)
```

The following images show robot models with opacity values of `1.0` and `0.5`.

| `opacity: 1` | `opacity: 0.5` |
|----|----|
|  |  |

## Topics

### Operators

static func == (OpacityComponent, OpacityComponent) -> Bool

Returns a Boolean value that indicates whether two opacity components are equal.

### Initializers

init(opacity: Float)

Creates a new opacity component.

### Instance Properties

var opacity: Float

The floating-point value the renderer applies to an entity and its descendants.

### Default Implementations

Component Implementations

Equatable Implementations

## Relationships

### Conforms To

- Component
- Equatable

## See Also

### Render configuration

struct ModelSortGroupComponent

A component that configures the rendering order for an entity’s model.

struct ModelSortGroup

A group that you assign to multiple entities to tell the renderer what order and how to render the entities in the group.

struct AdaptiveResolutionComponent

A component that provides the suggested pixels per meter necessary to render an object.

struct ModelDebugOptionsComponent

A component that changes how RealityKit renders its entity to help with debugging.

