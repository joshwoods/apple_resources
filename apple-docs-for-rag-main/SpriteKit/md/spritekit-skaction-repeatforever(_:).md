

- SpriteKit
- SKAction
-  repeatForever(\_:) 

Type Method

# repeatForever(\_:)

Creates an action that repeats another action forever.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class func repeatForever(_ action: SKAction) -> SKAction
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

### Chaining Actions

class func group([SKAction]) -> SKAction

Creates an action that runs a collection of actions in parallel.

class func sequence([SKAction]) -> SKAction

Creates an action that runs a collection of actions sequentially.

class func `repeat`(SKAction, count: Int) -> SKAction

Creates an action that repeats another action a specified number of times.

