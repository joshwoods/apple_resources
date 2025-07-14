

- RealityKit
- PointLightComponent
-  intensity 

Instance Property

# intensity

The intensity of the point light, measured in lumen.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS 2.0+

``` source
var intensity: Float
```

## Discussion

The default value is `26963.76` lumens.

See PointLightComponent for more information about how the `intensity` and attenuationRadius properties affect this light.

## See Also

### Configuring the light

var attenuationRadius: Float

The distance from the light source where its intensity reaches zero.

var attenuationFalloffExponent: Float

The exponent value for the light’s intensity falloff-transition curve.

