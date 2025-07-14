

- PHASE
- PHASESpatialPipelineEntry
-  sendLevelMetaParameterDefinition 

Instance Property

# sendLevelMetaParameterDefinition

A parameter that gradually updates the amount of audio signal that passes through to the output.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
var sendLevelMetaParameterDefinition: PHASENumberMetaParameterDefinition? { get set }
```

## Discussion

Use this property to fade reverb effects into a spatial mixer’s output.

For example, to begin with no reverb and gradually enable it, start by silencing reverb by setting the lateReverb entry’s sendLevel to `0`. Begin the fade by calling fade(value:duration:) on this property with an argument of `1`.

