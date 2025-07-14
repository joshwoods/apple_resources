

- SceneKit
- SCNAction
-  unhide() 

Type Method

# unhide()

Creates an action that ensures a node is not hidden.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class func unhide() -> SCNAction
```

## Return Value

A new action object.

## Discussion

When the action executes, the node’s isHidden property is set to false.

This action is reversible; the reverse is equivalent to the hide() action.

## See Also

### Creating Actions That Change a Node’s Visibility

class func hide() -> SCNAction

Creates an action that hides a node.

