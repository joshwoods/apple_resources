

- SceneKit
- SCNAction
-  move(by:duration:) 

Type Method

# move(by:duration:)

Creates an action that moves a node relative to its current position.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
class func move(
    by delta: SCNVector3,
    duration: TimeInterval
) -> SCNAction
```

## Parameters 

`delta`  

A vector that describes the change to be applied to the node’s position.

`duration`  

The duration, in seconds, of the animation.

## Return Value

A new action object.

## Discussion

When the action executes, the node’s position property animates from its current position to its new position.

This action is reversible; the reverse is created as if the following code had been executed:

```
SCNVector3 reverseDelta = SCNVector3Make(-delta.x, -delta.y, -delta.z);
[SCNAction moveBy: reverseDelta duration: duration];
```

## See Also

### Creating Actions That Move a Node

class func moveBy(x: CGFloat, y: CGFloat, z: CGFloat, duration: TimeInterval) -> SCNAction

Creates an action that moves a node relative to its current position.

class func move(to: SCNVector3, duration: TimeInterval) -> SCNAction

Creates an action that moves a node to a new position.

