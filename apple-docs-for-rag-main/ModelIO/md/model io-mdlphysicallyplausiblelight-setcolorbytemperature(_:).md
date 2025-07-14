

- Model I/O
- MDLPhysicallyPlausibleLight
-  setColorByTemperature(\_:) 

Instance Method

# setColorByTemperature(\_:)

Sets the light’s color based on a black-body temperature.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func setColorByTemperature(_ temperature: Float)
```

## Parameters 

`temperature`  

The black-body temperature, in Kelvins, whose luminous color the light should match.

## Discussion

Real-world light sources often measure color of illumination based on a black-body temperature scale. For example, the colors and characterizations of typical home and office light fixtures correspond to the following temperatures:

| Label           | Color                           | Temperature |
|-----------------|---------------------------------|-------------|
| “Soft white”    | Warm, yellowish white           | 2700 K      |
| “Bright white”  | Pale yellowish white            | 3000 K      |
| “Daylight”      | Bright, slightly greenish white | 5000 K      |
| “Cool daylight” | Bright, slightly bluish white   | 6500 K      |

## See Also

### Managing Light Color and Intensity

var color: CGColor?

The color of the light source.

var lumens: Float

The total visible intensity of the light source, in lumens.

