

- SceneKit
- SCNAction
-  removeFromParentNode() 

Type Method

# removeFromParentNode()

Creates an action that removes the node from its parent.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
class func removeFromParentNode() -> SCNAction
```

## Return Value

A new action object.

## Discussion

When the action executes, the node is immediately removed from its parent.

This action is not reversible; the reverse of this action is the same action.

