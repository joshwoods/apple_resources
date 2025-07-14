

- PHASE
- PHASESpatialPipeline
-  entries 

Instance Property

# entries

Audio layers for environmental effects to add to the output.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
var entries: [PHASESpatialCategory : PHASESpatialPipelineEntry] { get }
```

## Discussion

This property includes an entry for each spatial category that the app includes in the init(flags:) argument. Adjust an entry’s send level to blend its audio layer into the output signal. For example, by fading the input audio signal using the sendLevelMetaParameterDefinition property of the directPathTransmission entry, the app can lower the dry signal and blend in the right balance of early reflections and reverb.

## See Also

### Inspecting Effects

var flags: PHASESpatialPipeline.Flags

A collection of environmental effects to include in the output.

