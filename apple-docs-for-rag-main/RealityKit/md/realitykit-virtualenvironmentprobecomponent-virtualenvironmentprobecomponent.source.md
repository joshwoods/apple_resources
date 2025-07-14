

- RealityKit
- VirtualEnvironmentProbeComponent
-  VirtualEnvironmentProbeComponent.Source 

Enumeration

# VirtualEnvironmentProbeComponent.Source

Options that define the source of diffuse and specular lighting for environment lighting calculations.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
enum Source
```

## Topics

### Enumeration Cases

case blend(from: VirtualEnvironmentProbeComponent.Probe, to: VirtualEnvironmentProbeComponent.Probe, t: Float)

A source that blends between two pregenerated probes based on the provided blend factor.

case none

A source without any lighting.

case single(VirtualEnvironmentProbeComponent.Probe)

A source representing a single pregenerated probe.

## See Also

### Environment

class EnvironmentResource

An environmental resource that contains background and lighting information for a scene.

struct EnvironmentLightingConfigurationComponent

A component that scales the amount of light that an entity receives from its environment.

struct VirtualEnvironmentProbeComponent

A component that provides environment lighting for entities you place within the same virtual world.

struct Probe

A sample of the environment around a point in a scene the system uses for environment-based lighting.

