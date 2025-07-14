

- SpriteKit
-  SKActionTimingFunction 

Type Alias

# SKActionTimingFunction

The signature for the custom timing block.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
typealias SKActionTimingFunction = (Float) -> Float
```

## Discussion

The block parameters are defined as follows:

`time`  
The input time, where `0.0` represents the start time of the animation and `1.0` represents the end time of the animation.

The input value will be a value between `0.0` and `1.0`, inclusive. The block must also return a value between `0.0` and `1.0`. When the input time is `0.0`, the output value should be `0.0`. When the input time is `1.0`, the output value should also be `1.0`.

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

var speed: CGFloat

A speed factor that modifies how fast an action runs.

