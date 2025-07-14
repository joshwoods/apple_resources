

- RealityKit
- EnvironmentResource
- EnvironmentResource.CreateOptions
- EnvironmentResource.CreateOptions.SamplingQuality
-  EnvironmentResource.CreateOptions.SamplingQuality.fast 

Case

# EnvironmentResource.CreateOptions.SamplingQuality.fast

Computes the environment textures with small sampling rates.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
case fast
```

## Discussion

Low sampling rates can result in higher noise in high-frequency areas and banding in low-frequency gradients.

## See Also

### Sampling qualities

case normal

Computes the environment textures with regular sampling rates.

case high

Computes the environment textures with high sampling rates, reducing texture noise in high-frequency areas.

case veryHigh

Computes the environment textures with very high sampling rates.

