

- SpriteKit
- SKAction
-  wait(forDuration:) 

Type Method

# wait(forDuration:)

Creates an action that idles for a specified period of time.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class func wait(forDuration duration: TimeInterval) -> SKAction
```

## Parameters 

`duration`  

The amount of time to wait.

## Return Value

A new action object.

## Discussion

When the action executes, the action waits for the specified amount of time, then ends. This is typically used as part of a sequence of actions to insert a delay between two other actions. You might also use it in conjunction with the run(_:completion:) method to trigger code that needs to run at a later time.

This action is not reversible; the reverse of this action is the same action.

## See Also

### Delaying Actions

class func wait(forDuration: TimeInterval, withRange: TimeInterval) -> SKAction

Creates an action that idles for a randomized period of time.

