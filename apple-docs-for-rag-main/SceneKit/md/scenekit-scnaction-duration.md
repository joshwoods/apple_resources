

- SceneKit
- SCNAction
-  duration 

Instance Property

# duration

The duration required to complete an action.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var duration: TimeInterval { get set }
```

## Discussion

This is the expected duration of an action’s animation. The actual time an action takes to complete is modified by the action’s timingMode property.

## See Also

### Adjusting an Action’s Animation Properties

var speed: CGFloat

A speed factor that modifies how fast an action runs.

var timingMode: SCNActionTimingMode

The timing mode used to execute an action.

var timingFunction: SCNActionTimingFunction?

A block SceneKit calls to determine the action’s animation timing.

