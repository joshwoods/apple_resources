

- PHASE
- PHASEGeneratorNodeDefinition
-  rate 

Instance Property

# rate

A playback speed for the node’s audio.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
var rate: Double { get set }
```

## Discussion

The value clamps to the range `[0.25,` `4]`. The default value is `1`, which doesn’t change the source audio’s rate. Values higher than `1` speed up playback, and lower values slow it down.

## See Also

### Controlling Audio Playback

var rateMetaParameterDefinition: PHASENumberMetaParameterDefinition?

A meta parameter that dynamically changes the audio’s rate.

var gainMetaParameterDefinition: PHASENumberMetaParameterDefinition?

A meta parameter that dynamically changes the audio’s loudness.

