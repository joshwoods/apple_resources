

- SpriteKit
- SKAction
-  speed 

Instance Property

# speed

A speed factor that modifies how fast an action runs.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var speed: CGFloat { get set }
```

## Mentioned in 

Getting Started with Actions

## Discussion

The speed factor adjusts how fast an action’s animation runs. For example, a speed factor of `2.0` means the animation runs twice as fast.

## See Also

### Controlling Action Timing

Configuring Action Timing

Time an action in a scene, by adding or modifying timing properties, or cancel an action.

var duration: TimeInterval

The duration required to complete an action.

var timingMode: SKActionTimingMode

A setting that controls the speed curve of an animation.

enum SKActionTimingMode

The modes that an action can use to adjust the apparent timing of the action.

var timingFunction: SKActionTimingFunction

A block used to customize the timing function.

typealias SKActionTimingFunction

The signature for the custom timing block.

