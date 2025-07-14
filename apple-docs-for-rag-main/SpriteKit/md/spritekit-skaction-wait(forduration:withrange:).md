

- SpriteKit
- SKAction
-  wait(forDuration:withRange:) 

Type Method

# wait(forDuration:withRange:)

Creates an action that idles for a randomized period of time.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class func wait(
    forDuration duration: TimeInterval,
    withRange durationRange: TimeInterval
) -> SKAction
```

## Parameters 

`duration`  

The average amount of time to wait.

`durationRange`  

The range of possible values for the duration.

## Return Value

A new action object.

## Discussion

When the action executes, the action waits for the specified amount of time, then ends. This is typically used as part of a sequence of actions to insert a delay between two other actions. However, you might also use it in conjunction with the run(_:completion:) method to trigger code that needs to run at a later time.

Each time the action is executed, the action computes a new random value for the duration. The duration may vary in either direction by up to half of the value of the `durationRange` parameter.

This action is not reversible; the reverse of this action is the same action.

## See Also

### Delaying Actions

class func wait(forDuration: TimeInterval) -> SKAction

Creates an action that idles for a specified period of time.

