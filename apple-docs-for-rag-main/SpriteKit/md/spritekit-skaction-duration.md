

- SpriteKit
- SKAction
-  duration 

Instance Property

# duration

The duration required to complete an action.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var duration: TimeInterval { get set }
```

## Mentioned in 

Getting Started with Actions

## Discussion

This is the expected duration of an action’s animation. The actual time an action takes to complete is modified by the speed property of the action and the speed property of the node on which it executes.

## See Also

### Controlling Action Timing

Configuring Action Timing

Time an action in a scene, by adding or modifying timing properties, or cancel an action.

var timingMode: SKActionTimingMode

A setting that controls the speed curve of an animation.

enum SKActionTimingMode

The modes that an action can use to adjust the apparent timing of the action.

var timingFunction: SKActionTimingFunction

A block used to customize the timing function.

typealias SKActionTimingFunction

The signature for the custom timing block.

var speed: CGFloat

A speed factor that modifies how fast an action runs.

