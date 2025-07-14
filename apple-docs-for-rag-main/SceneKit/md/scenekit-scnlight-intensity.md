

- SceneKit
- SCNLight
-  intensity 

Instance Property

# intensity

The luminous flux, in lumens, or total brightness of the light. Animatable.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
var intensity: CGFloat { get set }
```

## Discussion

When working with photometric lights (see the iesProfileURL property) or physically-based rendering (see physicallyBased), you can leave the color property at its default white color and use the intensity and temperature to control the light using realistic parameters. When working with physically-based materials, this value the luminous flux of the light source. The default value is `1000` lumens.

When not using physically-based rendering, this value (divided by 1000) serves as a multiplier for the the color property. The default value of of `1000` leaves the light color unmodulated; you can use higher values, for example, to brighten a light whose color is already the maximum red value.

You can animate changes to this property’s value. See Animating SceneKit Content.

## See Also

### Modifying a Light’s Appearance

var type: SCNLight.LightType

A constant identifying the general behavior of the light.

struct LightType

Constants specifying the general behavior of a light, used by the type property.

var color: Any

The color of the light. Animatable.

var temperature: CGFloat

The color temperature, in degrees Kelvin, of the light source. Animatable.

var sphericalHarmonicsCoefficients: Data

Data describing the estimated lighting environment in all directions for a light probe.

