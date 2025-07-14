

- SceneKit
- SCNLight
-  attenuationFalloffExponent 

Instance Property

# attenuationFalloffExponent

The transition curve for the light’s intensity between its attenuation start and end distances. Animatable.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var attenuationFalloffExponent: CGFloat { get set }
```

## Discussion

You can apply attenuation to omnidirectional lights and spotlights, causing their intensity to diminish over a specified range of distances. At distances in between the start and end distance, the light’s intensity transitions from full to no illumination according to the value of this property.

A value of `0.0` specifies no attenuation—the light’s intensity is the same at all distances. A value of `1.0` specifies a linear transition, and a value of `2.0` (the default) specifies a quadratic transition curve. Higher values have little visible effect.

You can animate changes to this property’s value. See Animating SceneKit Content.

## See Also

### Managing Light Attenuation

var attenuationStartDistance: CGFloat

The distance from the light at which its intensity begins to diminish. Animatable.

var attenuationEndDistance: CGFloat

The distance from the light at which its intensity is completely diminished. Animatable.

