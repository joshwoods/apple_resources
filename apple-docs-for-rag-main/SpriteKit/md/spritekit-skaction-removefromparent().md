

- SpriteKit
- SKAction
-  removeFromParent() 

Type Method

# removeFromParent()

Creates an action that removes the node from its parent.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class func removeFromParent() -> SKAction
```

## Return Value

A new action object.

## Discussion

When the action executes, the node is immediately removed from its parent.

This action is not reversible; the reverse of this action is the same action.

