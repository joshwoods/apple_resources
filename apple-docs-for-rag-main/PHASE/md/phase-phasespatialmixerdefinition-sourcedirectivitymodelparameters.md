

- PHASE
- PHASESpatialMixerDefinition
-  sourceDirectivityModelParameters 

Instance Property

# sourceDirectivityModelParameters

A data set that directs sound such that it’s louder when directed at the listener.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
var sourceDirectivityModelParameters: PHASEDirectivityModelParameters? { get set }
```

## Discussion

The framework applies directivity to sound sources that emanate from a point.

## See Also

### Configuring Directivity

var listenerDirectivityModelParameters: PHASEDirectivityModelParameters?

A data set that determines how well the listener hears depending on its direction relative to a sound source.

