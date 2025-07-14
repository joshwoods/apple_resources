

- SceneKit
- SCNAction
-  moveBy(x:y:z:duration:) 

Type Method

# moveBy(x:y:z:duration:)

Creates an action that moves a node relative to its current position.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
class func moveBy(
    x deltaX: CGFloat,
    y deltaY: CGFloat,
    z deltaZ: CGFloat,
    duration: TimeInterval
) -> SCNAction
```

## Parameters 

`deltaX`  

The distance to move the node in the X direction of its parent node’s local coordinate space.

`deltaY`  

The distance to move the node in the Y direction of its parent node’s local coordinate space.

`deltaZ`  

The distance to move the node in the Z direction of its parent node’s local coordinate space.

`duration`  

The duration, in seconds, of the animation.

## Return Value

A new action object.

## Discussion

When the action executes, the node’s position property animates from its current position to its new position.

This action is reversible; the reverse is created as if the following code had been executed:

```
[SCNAction moveByX: -deltaX y: -deltaY z: -deltaZ duration: duration];
```

## See Also

### Creating Actions That Move a Node

class func move(by: SCNVector3, duration: TimeInterval) -> SCNAction

Creates an action that moves a node relative to its current position.

class func move(to: SCNVector3, duration: TimeInterval) -> SCNAction

Creates an action that moves a node to a new position.

