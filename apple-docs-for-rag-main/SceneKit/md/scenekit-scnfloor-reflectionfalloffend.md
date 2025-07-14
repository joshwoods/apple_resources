

- SceneKit
- SCNFloor
-  reflectionFalloffEnd 

Instance Property

# reflectionFalloffEnd

The distance from the floor at which scene contents are no longer reflected. Animatable.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var reflectionFalloffEnd: CGFloat { get set }
```

## Discussion

SceneKit can render reflections on a floor using an opacity gradient (or falloff). With this gradient, the reflections of scene contents closer to the floor are more visible than those of scene contents farther from it. This property marks the distance at which the opacity gradient ends. Scene contents farther away from the floor than this distance do not appear in the reflection.

If this property’s value is `0.0` (the default), SceneKit does not render the reflection with an opacity falloff—all scene contents are visible in the reflection regardless of their distance from the floor.

You can animate changes to this property’s value. See Animating SceneKit Content.

## See Also

### Adding Reflections to a Floor

var reflectivity: CGFloat

The intensity of the scene’s reflection on the floor. Animatable.

var reflectionFalloffStart: CGFloat

The distance from the floor at which scene contents are reflected at full intensity. Animatable.

var reflectionResolutionScaleFactor: CGFloat

The resolution scale factor of the offscreen buffer that SceneKit uses to render reflections.

var reflectionCategoryBitMask: Int

A mask that defines which categories of other objects show reflections on the floor.

