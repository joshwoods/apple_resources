

- SpriteKit
- SKAction
-  sequence(\_:) 

Type Method

# sequence(\_:)

Creates an action that runs a collection of actions sequentially.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class func sequence(_ actions: [SKAction]) -> SKAction
```

## Parameters 

`actions`  

An array of SKAction objects.

## Return Value

A sequence action object.

## Discussion

When the action executes, the first action in the sequence starts and runs to completion. Subsequent actions in the sequence run in a similar fashion until all of the actions in the sequence have executed. The duration of the sequence action is the sum of the durations of the actions in the sequence.

This action is reversible; it creates a new sequence action that reverses the order of the actions. Each action in the reversed sequence is itself reversed. For example, if an action sequence is `{1,2,3}`, the reversed sequence would be `{3R,2R,1R}`.

## See Also

### Chaining Actions

class func group([SKAction]) -> SKAction

Creates an action that runs a collection of actions in parallel.

class func `repeat`(SKAction, count: Int) -> SKAction

Creates an action that repeats another action a specified number of times.

class func repeatForever(SKAction) -> SKAction

Creates an action that repeats another action forever.

