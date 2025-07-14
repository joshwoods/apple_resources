

- SpriteKit
- SKAction
-  follow(\_:asOffset:orientToPath:speed:) 

Type Method

# follow(\_:asOffset:orientToPath:speed:)

Creates an action that moves the node at a specified speed along a path.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class func follow(
    _ path: CGPath,
    asOffset offset: Bool,
    orientToPath orient: Bool,
    speed: CGFloat
) -> SKAction
```

## Parameters 

`path`  

A path to follow.

`offset`  

If true, the points in the path are relative offsets to the node’s starting position. If false, the points in the node are absolute coordinate values.

`orient`  

If true, the node’s zRotation property animates so that the node turns to follow the path. If false, the zRotation property of the node is unchanged.

`speed`  

The speed at which the node should move, in points per second.

## Return Value

A new action object.

## Discussion

When the action executes, the node’s position and zRotation properties are animated along the provided path. The duration of the action is determined by the length of the path and the speed of the node.

This action is reversible; the resulting action creates a reversed path and then follows it, with the same speed.

## See Also

### Animating a Node’s Position Along a Custom Path

class func follow(CGPath, duration: TimeInterval) -> SKAction

Creates an action that moves the node along a relative path, orienting the node to the path.

class func follow(CGPath, speed: CGFloat) -> SKAction

Creates an action that moves the node along a relative path at a specified speed, orienting the node to the path.

class func follow(CGPath, asOffset: Bool, orientToPath: Bool, duration: TimeInterval) -> SKAction

Creates an action that moves the node along a path.

