

- SceneKit
- SCNShadowMode
-  SCNShadowMode.forward 

Case

# SCNShadowMode.forward

SceneKit renders shadows during lighting computations.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
case forward
```

## Discussion

In this mode, the color components of the light’s shadowColor property do not apply. The color’s alpha component determines the intensity of shadows.

## See Also

### Constants

case deferred

SceneKit renders shadows in a postprocessing pass.

case modulated

SceneKit renders shadows by projecting the light’s gobo image. The light does not illuminate the scene.

