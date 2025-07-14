

- SceneKit
- SCNLight
-  temperature 

Instance Property

# temperature

The color temperature, in degrees Kelvin, of the light source. Animatable.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
var temperature: CGFloat { get set }
```

## Discussion

SceneKit determines the actual color of the light by multiplying the color value by a color corresponding to the light’s temperature. The default value of `6500` K represents a pure white light (leaving the color unmodulated); lower values (down to a minimum of zero) add a “warmer” yellow or orange effect to the light source, and higher values (up to a maximum of `40000`) add a “cooler” blue effect.

This property affects all light types, but is especially useful when working with photometric lights (see the iesProfileURL property) or physically-based rendering (see physicallyBased). You can leave the color property at its default white color and use the intensity and temperature properties to control the light using realistic parameters.

You can animate changes to this property’s value. See Animating SceneKit Content.

## See Also

### Modifying a Light’s Appearance

var type: SCNLight.LightType

A constant identifying the general behavior of the light.

struct LightType

Constants specifying the general behavior of a light, used by the type property.

var color: Any

The color of the light. Animatable.

var intensity: CGFloat

The luminous flux, in lumens, or total brightness of the light. Animatable.

var sphericalHarmonicsCoefficients: Data

Data describing the estimated lighting environment in all directions for a light probe.

