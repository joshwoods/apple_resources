

- Model I/O
- MDLProbePlacement
-  MDLProbePlacement.irradianceDistribution 

Case

# MDLProbePlacement.irradianceDistribution

An option to examine the lighting conditions at various positions in the scene being evaluated, then place light probes only at the locations where each contributes optimally to scene lighting.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
case irradianceDistribution
```

## Discussion

If you use this heuristic, your data source must implement the sphericalHarmonicsCoefficients(atPosition:) method.

## See Also

### Constants

case uniformGrid

An option to place light probes at each unit coordinate in a three-dimensional grid that evenly divides the region being evaluated.

