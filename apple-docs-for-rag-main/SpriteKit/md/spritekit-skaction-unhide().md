

- SpriteKit
- SKAction
-  unhide() 

Type Method

# unhide()

Creates an action that makes a node visible.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
class func unhide() -> SKAction
```

## Return Value

A new action object.

## Discussion

This action has an instantaneous duration. When the action executes, the node’s isHidden property is set to false.

This action is reversible; the reversed action hides the node.

## See Also

### Controlling Node Visibility

class func hide() -> SKAction

Creates an action that hides a node.

