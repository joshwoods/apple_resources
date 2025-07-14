

- RealityKit
- EnvironmentResource
- EnvironmentResource.CreateOptions
- EnvironmentResource.CreateOptions.SamplingQuality
-  EnvironmentResource.CreateOptions.SamplingQuality.veryHigh 

Case

# EnvironmentResource.CreateOptions.SamplingQuality.veryHigh

Computes the environment textures with very high sampling rates.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
case veryHigh
```

## Discussion

Use only to capture very small frequency details in the specular texture.

Note

Only available in macOS.

## See Also

### Sampling qualities

case fast

Computes the environment textures with small sampling rates.

case normal

Computes the environment textures with regular sampling rates.

case high

Computes the environment textures with high sampling rates, reducing texture noise in high-frequency areas.

