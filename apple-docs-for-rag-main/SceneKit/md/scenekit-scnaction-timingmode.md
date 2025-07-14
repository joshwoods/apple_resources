

- SceneKit
- SCNAction
-  timingMode 

Instance Property

# timingMode

The timing mode used to execute an action.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var timingMode: SCNActionTimingMode { get set }
```

## Discussion

For possible values, see SCNActionTimingMode. The default value is SCNActionTimingMode.linear.

## See Also

### Adjusting an Action’s Animation Properties

var duration: TimeInterval

The duration required to complete an action.

var speed: CGFloat

A speed factor that modifies how fast an action runs.

var timingFunction: SCNActionTimingFunction?

A block SceneKit calls to determine the action’s animation timing.

