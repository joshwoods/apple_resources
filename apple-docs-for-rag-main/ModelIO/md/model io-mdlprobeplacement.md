

- Model I/O
-  MDLProbePlacement 

Enumeration

# MDLProbePlacement

Options affecting automatic placement of light probes in a scene, used with the placeLightProbes(withDensity:heuristic:using:) method.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
enum MDLProbePlacement
```

## Topics

### Constants

case irradianceDistribution

An option to examine the lighting conditions at various positions in the scene being evaluated, then place light probes only at the locations where each contributes optimally to scene lighting.

case uniformGrid

An option to place light probes at each unit coordinate in a three-dimensional grid that evenly divides the region being evaluated.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Working with Lights

class func placeLightProbes(withDensity: Float, heuristic: MDLProbePlacement, using: any MDLLightProbeIrradianceDataSource) -> [MDLLightProbe]

Automatically creates and places light probes for use in illuminating a scene.

