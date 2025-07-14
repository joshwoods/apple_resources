

- SceneKit
- SCNLight
-  color 

Instance Property

# color

The color of the light. Animatable.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var color: Any { get set }
```

## Discussion

The value of this property is an NSColor or CGColor object. The default color is white.

You can animate changes to this property’s value. See Animating SceneKit Content.

## See Also

### Modifying a Light’s Appearance

var type: SCNLight.LightType

A constant identifying the general behavior of the light.

struct LightType

Constants specifying the general behavior of a light, used by the type property.

var temperature: CGFloat

The color temperature, in degrees Kelvin, of the light source. Animatable.

var intensity: CGFloat

The luminous flux, in lumens, or total brightness of the light. Animatable.

var sphericalHarmonicsCoefficients: Data

Data describing the estimated lighting environment in all directions for a light probe.

