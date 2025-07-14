

- SpriteKit
- SKAction
-  hide() 

Type Method

# hide()

Creates an action that hides a node.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
class func hide() -> SKAction
```

## Return Value

A new action object.

## Discussion

This action has an instantaneous duration. When the action executes, the node’s isHidden property is set to true.

This action is reversible; the reversed action shows the node.

## See Also

### Controlling Node Visibility

class func unhide() -> SKAction

Creates an action that makes a node visible.

