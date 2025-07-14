

- SceneKit
- SCNShadowMode
-  SCNShadowMode.deferred 

Case

# SCNShadowMode.deferred

SceneKit renders shadows in a postprocessing pass.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
case deferred
```

## Discussion

In the mode, SceneKit blends shadows into the final image after the main rendering pass, so shadows can be of any color.

## See Also

### Constants

case forward

SceneKit renders shadows during lighting computations.

case modulated

SceneKit renders shadows by projecting the light’s gobo image. The light does not illuminate the scene.

