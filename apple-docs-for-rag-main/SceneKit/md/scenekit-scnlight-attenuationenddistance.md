

- SceneKit
- SCNLight
-  attenuationEndDistance 

Instance Property

# attenuationEndDistance

The distance from the light at which its intensity is completely diminished. Animatable.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var attenuationEndDistance: CGFloat { get set }
```

## Discussion

You can apply attenuation to omnidirectional lights and spotlights, causing their intensity to diminish over a specified range of distances. At distances less than the start distance, the light’s illumination is at full intensity. At distances greater than the end distance, the light provides no illumination. At distances in between the start and end distance, the attenuationFalloffExponent property defines the transition from full illumination to no illumination.

The default value is `0.0`, specifying no attenuation (the light’s intensity is the same at all distances).

You can animate changes to this property’s value. See Animating SceneKit Content.

## See Also

### Managing Light Attenuation

var attenuationStartDistance: CGFloat

The distance from the light at which its intensity begins to diminish. Animatable.

var attenuationFalloffExponent: CGFloat

The transition curve for the light’s intensity between its attenuation start and end distances. Animatable.

