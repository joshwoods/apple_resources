

- RealityKit
-  VirtualEnvironmentProbeComponent 

Structure

# VirtualEnvironmentProbeComponent

A component that provides environment lighting for entities you place within the same virtual world.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
struct VirtualEnvironmentProbeComponent
```

## Overview

In a fully virtual environment, you can configure the `VirtualEnvironmentProbeComponent` with an EnvironmentResource to provide precalculated indirect lighting from the environment. RealityKit combines this lighting with other lights in the scene to calculate the final lighting of an entity. The example below shows how you can set up a `VirtualEnvironmentProbeComponent` from a single probe:

```
let environment = try await Entity(named: "environment")
let resource = try await EnvironmentResource(named: "MyEnvironment", in: bundle)
let probe = VirtualEnvironmentProbeComponent.Probe(environment: resource)
let probeComponent = VirtualEnvironmentProbeComponent(source: .single(probe))
environment.components.set(probeComponent)
```

Note

In visionOS, ARKit automatically provides the environment lighting for the shared space.

## Topics

### Structures

struct Probe

A sample of the environment around a point in a scene the system uses for environment-based lighting.

### Initializers

init(source: VirtualEnvironmentProbeComponent.Source)

Creates a virtual-environment probe component.

### Instance Properties

var source: VirtualEnvironmentProbeComponent.Source

The source of diffuse and specular lighting for environment lighting calculations.

### Enumerations

enum Source

Options that define the source of diffuse and specular lighting for environment lighting calculations.

### Default Implementations

Component Implementations

## Relationships

### Conforms To

- Component

## See Also

### Environment

class EnvironmentResource

An environmental resource that contains background and lighting information for a scene.

struct EnvironmentLightingConfigurationComponent

A component that scales the amount of light that an entity receives from its environment.

struct Probe

A sample of the environment around a point in a scene the system uses for environment-based lighting.

enum Source

Options that define the source of diffuse and specular lighting for environment lighting calculations.

