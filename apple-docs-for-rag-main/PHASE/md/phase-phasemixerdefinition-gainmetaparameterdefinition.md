

- PHASE
- PHASEMixerDefinition
-  gainMetaParameterDefinition 

Instance Property

# gainMetaParameterDefinition

A template for a parameter that changes the mixer’s volume gradually over a period of time.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
var gainMetaParameterDefinition: PHASENumberMetaParameterDefinition? { get set }
```

## Discussion

When the framework creates a mixer from a mixer definition, PHASE initializes the mixer’s gainMetaParameter to this property’s values.

## See Also

### Controlling Volume

var gain: Double

The mixer’s volume.

