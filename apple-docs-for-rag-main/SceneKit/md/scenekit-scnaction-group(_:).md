

- SceneKit
- SCNAction
-  group(\_:) 

Type Method

# group(\_:)

Creates an action that runs a collection of actions in parallel.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
class func group(_ actions: [SCNAction]) -> SCNAction
```

## Parameters 

`actions`  

An array of SCNAction objects.

## Return Value

A new group action object.

## Discussion

When the action executes, the actions that make up the group all start immediately and run in parallel. The duration of the group action is the longest duration among the collection of actions. If an action in the group has a duration less than the group’s duration, the action completes and then idles until the group completes the remaining actions. This matters most when creating a repeating action that repeats a group.

This action is reversible; it creates a new group action that contains the reverse of each action specified in the group.

## See Also

### Creating Actions That Combine or Repeat Other Actions

class func sequence([SCNAction]) -> SCNAction

Creates an action that runs a collection of actions sequentially.

class func `repeat`(SCNAction, count: Int) -> SCNAction

Creates an action that repeats another action a specified number of times.

class func repeatForever(SCNAction) -> SCNAction

Creates an action that repeats another action forever.

