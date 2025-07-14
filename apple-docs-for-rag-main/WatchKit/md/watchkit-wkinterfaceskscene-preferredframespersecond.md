

- WatchKit
- WKInterfaceSKScene
-  preferredFramesPerSecond 

Instance Property

# preferredFramesPerSecond

The animation frame rate that the interface uses to render its scene.

watchOS 3.0+

``` source
var preferredFramesPerSecond: Int { get set }
```

## Mentioned in 

Configuring a WatchKit Scene in a Storyboard

## Discussion

SpriteKit chooses an actual frame rate that is as close as possible to your preferred frame rate based on the capabilities of the hardware and the systems other requirements. Choose a frame rate that your app can consistently maintain. The default value is 60 frames per second.

To provide a consistent frame rate, SpriteKit usually selects a frame rate that is a factor of the hardware’s maximum refresh rate. For example, if Apple Watch’s maximum refresh rate is 60 frames per second, then that is also the highest frame rate used by SpriteKit. However, if you ask for a lower frame rate, SpriteKit might choose 30, 20, 15 or some other factor as the actual frame rate.

## See Also

### Controlling the Timing of a Scene’s Rendering

var isPaused: Bool

A Boolean value that determines whether the view’s scene animations are paused.

