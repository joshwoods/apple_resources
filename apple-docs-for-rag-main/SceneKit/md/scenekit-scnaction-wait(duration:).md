

- SceneKit
- SCNAction
-  wait(duration:) 

Type Method

# wait(duration:)

Creates an action that idles for a specified period of time.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
class func wait(duration sec: TimeInterval) -> SCNAction
```

## Parameters 

`sec`  

The amount of time to wait.

## Return Value

A new action object.

## Discussion

When the action executes, the action waits for the specified amount of time and then ends. This is typically used as part of a sequence of actions to insert a delay between two other actions. You might also use it in conjunction with the runAction(_:completionHandler:) method to trigger code that needs to run at a later time.

This action is not reversible; the reverse of this action is the same action.

## See Also

### Creating Actions That Add Delays to Action Sequences

class func wait(duration: TimeInterval, withRange: TimeInterval) -> SCNAction

Creates an action that idles for a randomized period of time.

