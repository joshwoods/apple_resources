

- SceneKit
-  SCNActionTimingFunction 

Type Alias

# SCNActionTimingFunction

The signature for a block that manages animation timing, used by the timingFunction property.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
typealias SCNActionTimingFunction = (Float) -> Float
```

## Discussion

The block takes a single parameter:

time  
A fraction of the action’s The input value for the timing function, as determined by the timingMode property and the action’s current progress.

Your block must return a floating-point value between `0.0` and `1.0`, where `0.0` represents the starting state of the action’s animation and `1.0` represents the end state.

## See Also

### Constants

enum SCNActionTimingMode

Constants affecting the animation curve of an action, used by the timingMode property.

