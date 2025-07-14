

- SpriteKit
- SKAction
-  repeat(\_:count:) 

Type Method

# repeat(\_:count:)

Creates an action that repeats another action a specified number of times.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class func `repeat`(
    _ action: SKAction,
    count: Int
) -> SKAction
```

## Parameters 

`action`  

The action to execute.

`count`  

The number of times to execute the action.

## Return Value

A new action object.

## Discussion

When the action executes, the associated action runs to completion and then repeats, until the count is reached.

This action is reversible; it creates a new action that is the reverse of the specified action and then repeats it the same number of times.

## See Also

### Chaining Actions

class func group([SKAction]) -> SKAction

Creates an action that runs a collection of actions in parallel.

class func sequence([SKAction]) -> SKAction

Creates an action that runs a collection of actions sequentially.

class func repeatForever(SKAction) -> SKAction

Creates an action that repeats another action forever.

