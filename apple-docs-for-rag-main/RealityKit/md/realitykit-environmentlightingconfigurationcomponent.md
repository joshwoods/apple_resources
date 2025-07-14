

- RealityKit
-  EnvironmentLightingConfigurationComponent 

Structure

# EnvironmentLightingConfigurationComponent

A component that scales the amount of light that an entity receives from its environment.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
struct EnvironmentLightingConfigurationComponent
```

## Overview

When rendering a RealityKit scene, you can control how much the environment’s lighting affects the virtual objects in your scene, such as the lighting from your real-world surroundings, a virtual environment, or both. Use an `EnvironmentLightingConfigurationComponent` to configure this amount for an entity.

For example, create an entity that receives no lighting from its environment by setting the weight to `0.0`.

```
let spaceship = try await Entity(named: "spaceship")
spaceship.components.set(EnvironmentLightingConfigurationComponent(
    environmentLightingWeight: 0.0))
```

Note

The weight value of the component also affects the lighting of the entity’s descendants.

## Topics

### Creating an environment-lighting configuration component

init(environmentLightingWeight: Float)

Creates an environment-lighting configuration component.

### Scaling the environment-lighting contribution

var environmentLightingWeight: Float

A value that controls the environment-lighting contribution to an entity’s lighting.

### Comparing environment-lighting configuration components

static func == (EnvironmentLightingConfigurationComponent, EnvironmentLightingConfigurationComponent) -> Bool

Returns a Boolean value that indicates whether two environment-lighting configuration components are equal.

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

### Default Implementations

Component Implementations

Equatable Implementations

## Relationships

### Conforms To

- Component
- Equatable

## See Also

### Environment

class EnvironmentResource

An environmental resource that contains background and lighting information for a scene.

struct VirtualEnvironmentProbeComponent

A component that provides environment lighting for entities you place within the same virtual world.

struct Probe

A sample of the environment around a point in a scene the system uses for environment-based lighting.

enum Source

Options that define the source of diffuse and specular lighting for environment lighting calculations.

