

- RealityKit
- PointLightComponent
-  attenuationRadius 

Instance Property

# attenuationRadius

The distance from the light source where its intensity reaches zero.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS 2.0+

``` source
var attenuationRadius: Float
```

## Discussion

Any objects at or beyond this distance do not receive illumination. The default value is `10.0` meters.

See PointLightComponent for more information about how the intensity and `attenuationRadius` properties affect this light.

## See Also

### Configuring the light

var intensity: Float

The intensity of the point light, measured in lumen.

var attenuationFalloffExponent: Float

The exponent value for the light’s intensity falloff-transition curve.

