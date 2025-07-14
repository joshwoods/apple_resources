

- PHASE
- PHASESpatialMixerDefinition
-  listenerDirectivityModelParameters 

Instance Property

# listenerDirectivityModelParameters

A data set that determines how well the listener hears depending on its direction relative to a sound source.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
var listenerDirectivityModelParameters: PHASEDirectivityModelParameters? { get set }
```

## Discussion

An app can configure this property to attenuate sound to the sides of the listener while leaving sound in front of or behind the listener unchanged.

## See Also

### Configuring Directivity

var sourceDirectivityModelParameters: PHASEDirectivityModelParameters?

A data set that directs sound such that it’s louder when directed at the listener.

