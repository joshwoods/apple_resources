

- PHASE
- PHASEMixer
-  gainMetaParameter 

Instance Property

# gainMetaParameter

A parameter that changes the mixer’s volume gradually over a period of time.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
var gainMetaParameter: PHASEMetaParameter? { get }
```

## Discussion

Use this property to smoothly adjust the volume of the mixer’s audio signals by calling fade(value:duration:).

The framework sets the initial value of this property according to the metaparameter definition object’s gainMetaParameterDefinition.

## See Also

### Adjusting Volume

var gain: Double

The mixer’s volume.

