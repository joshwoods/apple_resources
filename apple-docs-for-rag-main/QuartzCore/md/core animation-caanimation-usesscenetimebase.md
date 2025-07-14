

- Core Animation
- CAAnimation
-  usesSceneTimeBase 

Instance Property

# usesSceneTimeBase

For animations attached to SceneKit objects, a Boolean value that determines whether the animation is evaluated using the scene time or the system time.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
var usesSceneTimeBase: Bool { get set }
```

## Discussion

If the value of this property is true, animation timing is governed by the currentTime property of the view, layer, or custom renderer responsible for drawing the scene. The default value is false.

To attach animations to SceneKit objects, see SCNAnimatable.

