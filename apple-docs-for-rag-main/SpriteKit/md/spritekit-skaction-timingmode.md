

- SpriteKit
- SKAction
-  timingMode 

Instance Property

# timingMode

A setting that controls the speed curve of an animation.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var timingMode: SKActionTimingMode { get set }
```

## Mentioned in 

Configuring Action Timing

Getting Started with Actions

## Discussion

The possible values for this property are listed in SKActionTimingMode. The default value is SKActionTimingMode.linear.

## See Also

### Controlling Action Timing

Configuring Action Timing

Time an action in a scene, by adding or modifying timing properties, or cancel an action.

var duration: TimeInterval

The duration required to complete an action.

enum SKActionTimingMode

The modes that an action can use to adjust the apparent timing of the action.

var timingFunction: SKActionTimingFunction

A block used to customize the timing function.

typealias SKActionTimingFunction

The signature for the custom timing block.

var speed: CGFloat

A speed factor that modifies how fast an action runs.

