

- RealityKit
- EnvironmentResource
- EnvironmentResource.CreateOptions
-  EnvironmentResource.CreateOptions.SamplingQuality 

Enumeration

# EnvironmentResource.CreateOptions.SamplingQuality

An object for controlling the skybox sampling quality for lighting textures.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
enum SamplingQuality
```

## Topics

### Sampling qualities

case fast

Computes the environment textures with small sampling rates.

case normal

Computes the environment textures with regular sampling rates.

case high

Computes the environment textures with high sampling rates, reducing texture noise in high-frequency areas.

case veryHigh

Computes the environment textures with very high sampling rates.

### Comparing sampling quality

static func == (EnvironmentResource.CreateOptions.SamplingQuality, EnvironmentResource.CreateOptions.SamplingQuality) -> Bool

Returns a Boolean value indicating whether two values are equal.

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

var hashValue: Int

The hash value.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable
- Hashable
- Sendable

