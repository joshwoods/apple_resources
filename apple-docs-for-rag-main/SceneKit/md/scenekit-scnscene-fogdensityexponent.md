

- SceneKit
- SCNScene
-  fogDensityExponent 

Instance Property

# fogDensityExponent

The transition curve for the fog’s intensity between its start and end distances. Animatable.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var fogDensityExponent: CGFloat { get set }
```

## Discussion

A fog effect fades out the contents of the scene with increasing distance from the pointOfView location, replacing them with increasing intensities of the fogColor color. The fogDensityExponent property determines the smoothness or abruptness of this transition.

A value of `0.0` (the default) specifies no attenuation—the fog’s intensity is the same at all distances . A value of `1.0` specifies a linear transition, and a value of `2.0` specifies a quadratic transition curve. Higher values have little visible effect.

You can animate changes to this property’s value. See Animating SceneKit Content.

## See Also

### Adding Fog to a Scene

var fogStartDistance: CGFloat

The distance from a point of view at which the scene’s contents begin to be obscured by fog. Animatable.

var fogEndDistance: CGFloat

The distance from a point of view at which the scene’s contents are completely obscured by fog. Animatable.

var fogColor: Any

The color of the fog effect to be rendered with the scene. Animatable.

