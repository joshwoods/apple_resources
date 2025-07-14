

- SceneKit
- SCNAction
-  wait(duration:withRange:) 

Type Method

# wait(duration:withRange:)

Creates an action that idles for a randomized period of time.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
class func wait(
    duration sec: TimeInterval,
    withRange durationRange: TimeInterval
) -> SCNAction
```

## Parameters 

`sec`  

The average amount of time to wait.

`durationRange`  

The range of possible values for the duration.

## Return Value

A new action object.

## Discussion

When the action executes, the action waits for the specified amount of time and then ends. This is typically used as part of a sequence of actions to insert a delay between two other actions. However, you might also use it in conjunction with the runAction(_:completionHandler:) method to trigger code that needs to run at a later time.

Each time the action is executed, the action computes a new random value for the duration. The duration may vary in either direction by up to half of the value of the `durationRange` parameter.

This action is not reversible; the reverse of this action is the same action.

## See Also

### Creating Actions That Add Delays to Action Sequences

class func wait(duration: TimeInterval) -> SCNAction

Creates an action that idles for a specified period of time.

