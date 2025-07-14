

- SceneKit
- SCNAction
-  repeat(\_:count:) 

Type Method

# repeat(\_:count:)

Creates an action that repeats another action a specified number of times.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
class func `repeat`(
    _ action: SCNAction,
    count: Int
) -> SCNAction
```

## Parameters 

`action`  

The action to be executed.

`count`  

The number of times to execute the action.

## Return Value

A new action object.

## Discussion

When the action executes, the associated action runs to completion and then repeats, until the count is reached.

This action is reversible; it creates a new action that is the reverse of the specified action and then repeats it the same number of times.

## See Also

### Creating Actions That Combine or Repeat Other Actions

class func group([SCNAction]) -> SCNAction

Creates an action that runs a collection of actions in parallel.

class func sequence([SCNAction]) -> SCNAction

Creates an action that runs a collection of actions sequentially.

class func repeatForever(SCNAction) -> SCNAction

Creates an action that repeats another action forever.

