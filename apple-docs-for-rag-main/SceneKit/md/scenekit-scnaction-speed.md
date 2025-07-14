

- SceneKit
- SCNAction
-  speed 

Instance Property

# speed

A speed factor that modifies how fast an action runs.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var speed: CGFloat { get set }
```

## Discussion

The speed factor adjusts how fast an action’s animation runs. For example, a speed factor of `2.0` means the animation runs twice as fast.

## See Also

### Adjusting an Action’s Animation Properties

var duration: TimeInterval

The duration required to complete an action.

var timingMode: SCNActionTimingMode

The timing mode used to execute an action.

var timingFunction: SCNActionTimingFunction?

A block SceneKit calls to determine the action’s animation timing.

