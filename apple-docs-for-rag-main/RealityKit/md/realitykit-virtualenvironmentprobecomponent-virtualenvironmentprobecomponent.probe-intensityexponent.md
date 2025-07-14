

- RealityKit
- VirtualEnvironmentProbeComponent
- VirtualEnvironmentProbeComponent.Probe
-  intensityExponent 

Instance Property

# intensityExponent

The intensity value for the resource, which RealityKit defines on a logarithmic scale.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
var intensityExponent: Float
```

## Discussion

RealityKit multiplies the intensity of the probe by `2^intensityExponent`. An `intensityExponent` of `0.0` means using the diffuse and specular intensities as-is.

