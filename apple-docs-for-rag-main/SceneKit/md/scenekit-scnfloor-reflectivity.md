

- SceneKit
- SCNFloor
-  reflectivity 

Instance Property

# reflectivity

The intensity of the scene’s reflection on the floor. Animatable.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var reflectivity: CGFloat { get set }
```

## Discussion

If this property’s value is greater than zero, SceneKit renders a reflection for all contents of the scene located above the floor.

A lower reflectivity causes the rendered reflection to appear with less intensity, allowing the floor’s material to be more visible. At higher reflectivity values, the rendered reflection appears with greater intensity than the floor’s own material. The default reflectivity is `0.25`.

You can animate changes to this property’s value. See Animating SceneKit Content.

## See Also

### Adding Reflections to a Floor

var reflectionFalloffEnd: CGFloat

The distance from the floor at which scene contents are no longer reflected. Animatable.

var reflectionFalloffStart: CGFloat

The distance from the floor at which scene contents are reflected at full intensity. Animatable.

var reflectionResolutionScaleFactor: CGFloat

The resolution scale factor of the offscreen buffer that SceneKit uses to render reflections.

var reflectionCategoryBitMask: Int

A mask that defines which categories of other objects show reflections on the floor.

