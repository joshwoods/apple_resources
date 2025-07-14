

- WatchKit
- WKInterfaceSKScene
-  isPaused 

Instance Property

# isPaused

A Boolean value that determines whether the view’s scene animations are paused.

watchOS 3.0+

``` source
var isPaused: Bool { get set }
```

## Mentioned in 

Configuring a WatchKit Scene in a Storyboard

## Discussion

If the value is true, the scene’s content is fixed onscreen. No actions are executed and no physics simulation is performed.

## See Also

### Controlling the Timing of a Scene’s Rendering

var preferredFramesPerSecond: Int

The animation frame rate that the interface uses to render its scene.

