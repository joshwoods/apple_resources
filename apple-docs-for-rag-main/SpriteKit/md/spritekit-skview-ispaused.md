

- SpriteKit
- SKView
-  isPaused 

Instance Property

# isPaused

A Boolean value that indicates whether the view’s scene animations are paused.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
@MainActor
var isPaused: Bool { get set }
```

## Discussion

If the value is true, the scene’s content is fixed onscreen. No actions are executed and no physics simulation is performed.

When an application moves from an active to an inactive state, isPaused is automatically set to true. When an application returns to an active state, isPaused is automatically set to its previous value.

## See Also

### Controlling the Timing of a Scene’s Rendering

var preferredFramesPerSecond: Int

The animation frame rate that the view uses to render its scene.

var delegate: (any SKViewDelegate)?

A delegate that allows dynamic control of the view’s render rate.

protocol SKViewDelegate

Methods to take custom control over the view’s render rate.

var frameInterval: Int

The number of frames that must pass before the scene is called to update its contents.

Deprecated

var preferredFrameRate: FloatDeprecated

