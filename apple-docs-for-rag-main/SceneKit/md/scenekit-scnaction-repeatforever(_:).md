

- SceneKit
- SCNAction
-  repeatForever(\_:) 

Type Method

# repeatForever(\_:)

Creates an action that repeats another action forever.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
class func repeatForever(_ action: SCNAction) -> SCNAction
```

## Parameters 

`action`  

The action to execute.

## Return Value

A new action object.

## Discussion

When the action executes, the associated action runs to completion and then repeats.

This action is reversible; it creates a new action that is the reverse of the specified action and then repeats it forever.

Note

The action to be repeated must have a non-instantaneous duration.

## See Also

### Creating Actions That Combine or Repeat Other Actions

class func group([SCNAction]) -> SCNAction

Creates an action that runs a collection of actions in parallel.

class func sequence([SCNAction]) -> SCNAction

Creates an action that runs a collection of actions sequentially.

class func `repeat`(SCNAction, count: Int) -> SCNAction

Creates an action that repeats another action a specified number of times.

