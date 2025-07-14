

- SceneKit
- SCNAction
-  timingFunction 

Instance Property

# timingFunction

A block SceneKit calls to determine the action’s animation timing.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var timingFunction: SCNActionTimingFunction? { get set }
```

## Discussion

The timingMode property determines the input to your block. You use this input to compute your custom timing function, whose output determines the animation timing. The following example provides quadratic animation timing for an action, simulating the effect of gravity on a falling object:

```
action.timingMode = SCNActionTimingModeLinear;
action.timingFunction = ^float(float time) {
    return 1.0 - time*time;
};
```

## See Also

### Adjusting an Action’s Animation Properties

var duration: TimeInterval

The duration required to complete an action.

var speed: CGFloat

A speed factor that modifies how fast an action runs.

var timingMode: SCNActionTimingMode

The timing mode used to execute an action.

