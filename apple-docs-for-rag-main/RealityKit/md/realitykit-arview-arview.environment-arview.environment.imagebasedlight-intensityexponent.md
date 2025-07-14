

- RealityKit
- ARView
- ARView.Environment
- ARView.Environment.ImageBasedLight
-  intensityExponent 

Instance Property

# intensityExponent

The intensity value of the light, defined on a logarithmic scale.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+

``` source
var intensityExponent: Float
```

## Discussion

An intensity factor is computed as `2^intensityExponent`. The computed value modulates the native value specified in the diffuse and specular textures.

Set the intensity to `0` to result in a scale factor of `1`. This uses the unmodified texture’s diffuse and specular intensities.

