

- SceneKit
- SCNShadowMode
-  SCNShadowMode.modulated 

Case

# SCNShadowMode.modulated

SceneKit renders shadows by projecting the light’s gobo image. The light does not illuminate the scene.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
case modulated
```

## Discussion

Typically, you use this mode to create a low-accuracy, high-performance shadow under a game character or similar scene element: Use an image of a radial gradient (black to white) for the light’s gobo property, and use categoryBitMask properties to prevent the shadow image from appearing on the character.

## See Also

### Constants

case forward

SceneKit renders shadows during lighting computations.

case deferred

SceneKit renders shadows in a postprocessing pass.

