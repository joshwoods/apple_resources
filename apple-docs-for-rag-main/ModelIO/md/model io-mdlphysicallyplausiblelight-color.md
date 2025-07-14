

- Model I/O
- MDLPhysicallyPlausibleLight
-  color 

Instance Property

# color

The color of the light source.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var color: CGColor? { get set }
```

## Discussion

The default color corresponds to a color temperature of 6500 K, as described by the setColorByTemperature(_:) method.

## See Also

### Managing Light Color and Intensity

var lumens: Float

The total visible intensity of the light source, in lumens.

func setColorByTemperature(Float)

Sets the light’s color based on a black-body temperature.

