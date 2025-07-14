

- SceneKit
- SCNAction
-  sequence(\_:) 

Type Method

# sequence(\_:)

Creates an action that runs a collection of actions sequentially.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
class func sequence(_ actions: [SCNAction]) -> SCNAction
```

## Parameters 

`actions`  

An array of SCNAction objects.

## Return Value

A new sequence action object.

## Discussion

When the action executes, the first action in the sequence starts and runs to completion. Subsequent actions in the sequence run in a similar fashion until all of the actions in the sequence have executed. The duration of the sequence action is the sum of the durations of the actions in the sequence.

This action is reversible; it creates a new sequence action that reverses the order of the actions. Each action in the reversed sequence is itself reversed. For example, the actions `reverseSequence` and `sequenceReverse` in the code example below are equivalent:

```
SCNAction *sequence = [SCNAction sequence:@[ actionA, actionB, actionC ]];
SCNAction *reverseSequence = [SCNAction sequence:@[ [actionC reversedAction],
                                                    [actionB reversedAction],
                                                    [actionA reversedAction] ]];
SCNAction *sequenceReverse = [sequence reversedAction];
```

## See Also

### Creating Actions That Combine or Repeat Other Actions

class func group([SCNAction]) -> SCNAction

Creates an action that runs a collection of actions in parallel.

class func `repeat`(SCNAction, count: Int) -> SCNAction

Creates an action that repeats another action a specified number of times.

class func repeatForever(SCNAction) -> SCNAction

Creates an action that repeats another action forever.

