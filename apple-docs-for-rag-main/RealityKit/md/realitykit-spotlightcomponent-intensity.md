

- RealityKit
- SpotLightComponent
-  intensity 

Instance Property

# intensity

The intensity of the spotlight measured in lumen.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS 2.0+

``` source
var intensity: Float
```

## Discussion

The default value is `6740.94` lumens.

For more information on how the `intensity` and attenuationRadius affect this light, see SpotLightComponent.

## See Also

### Configuring the spotlight

var innerAngleInDegrees: Float

The inner angle of the spotlight in degrees.

var outerAngleInDegrees: Float

The outer angle of the spotlight in degrees.

var attenuationRadius: Float

The distance from the light source where its intensity reaches zero.

var attenuationFalloffExponent: Float

The exponent value for the light’s intensity falloff-transition curve.

