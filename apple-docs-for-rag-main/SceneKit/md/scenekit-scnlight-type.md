

- SceneKit
- SCNLight
-  type 

Instance Property

# type

A constant identifying the general behavior of the light.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var type: SCNLight.LightType { get set }
```

## Discussion

A light’s type determines the shape and directionality of illumination provided by the light, as well as the set of attributes available for modifying the light’s behavior. For example, light types include omnidirectional lights and spotlights. See `Light Types` for the full set of types and their behaviors.

## See Also

### Modifying a Light’s Appearance

struct LightType

Constants specifying the general behavior of a light, used by the type property.

var color: Any

The color of the light. Animatable.

var temperature: CGFloat

The color temperature, in degrees Kelvin, of the light source. Animatable.

var intensity: CGFloat

The luminous flux, in lumens, or total brightness of the light. Animatable.

var sphericalHarmonicsCoefficients: Data

Data describing the estimated lighting environment in all directions for a light probe.

