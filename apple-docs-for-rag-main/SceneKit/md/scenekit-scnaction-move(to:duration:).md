

- SceneKit
- SCNAction
-  move(to:duration:) 

Type Method

# move(to:duration:)

Creates an action that moves a node to a new position.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
class func move(
    to location: SCNVector3,
    duration: TimeInterval
) -> SCNAction
```

## Parameters 

`location`  

The coordinates for the node’s new position in its parent node’s local coordinate space.

`duration`  

The duration, in seconds, of the animation.

## Return Value

A new action object.

## Discussion

When the action executes, the node’s position property animates from its current position to its new position.

This action is not reversible; the reverse of this action has the same duration but does not move the node.

## See Also

### Creating Actions That Move a Node

class func moveBy(x: CGFloat, y: CGFloat, z: CGFloat, duration: TimeInterval) -> SCNAction

Creates an action that moves a node relative to its current position.

class func move(by: SCNVector3, duration: TimeInterval) -> SCNAction

Creates an action that moves a node relative to its current position.

