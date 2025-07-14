

- Model I/O
- MDLPhysicallyPlausibleLight
-  lumens 

Instance Property

# lumens

The total visible intensity of the light source, in lumens.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var lumens: Float { get set }
```

## Discussion

The default intensity is 1000 lumens.

## See Also

### Managing Light Color and Intensity

var color: CGColor?

The color of the light source.

func setColorByTemperature(Float)

Sets the light’s color based on a black-body temperature.

