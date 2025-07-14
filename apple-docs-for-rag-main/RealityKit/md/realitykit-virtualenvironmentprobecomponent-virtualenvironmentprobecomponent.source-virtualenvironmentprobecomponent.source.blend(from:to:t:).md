

- RealityKit
- VirtualEnvironmentProbeComponent
- VirtualEnvironmentProbeComponent.Source
-  VirtualEnvironmentProbeComponent.Source.blend(from:to:t:) 

Case

# VirtualEnvironmentProbeComponent.Source.blend(from:to:t:)

A source that blends between two pregenerated probes based on the provided blend factor.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
case blend(
    from: VirtualEnvironmentProbeComponent.Probe,
    to: VirtualEnvironmentProbeComponent.Probe,
    t: Float
)
```

## Discussion

The blend factor is in the range `[0.0, 1.0]` where a value of `0.0` uses only the first probe, and `1.0` uses only the second probe.

