

- SpriteKit
- SKAction
-  follow(\_:duration:) 

Type Method

# follow(\_:duration:)

Creates an action that moves the node along a relative path, orienting the node to the path.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class func follow(
    _ path: CGPath,
    duration: TimeInterval
) -> SKAction
```

## Parameters 

`path`  

A Core Graphics path whose coordinates are relative to the node’s current position.

`duration`  

The duration of the animation.

## Return Value

A new action object.

## Discussion

Calling this method is equivalent to calling the follow(_:asOffset:orientToPath:duration:) method, passing in true to both the `offset` and `orient` parameters.

This action is reversible; the resulting action creates and then follows a reversed path with the same duration.

## See Also

### Animating a Node’s Position Along a Custom Path

class func follow(CGPath, speed: CGFloat) -> SKAction

Creates an action that moves the node along a relative path at a specified speed, orienting the node to the path.

class func follow(CGPath, asOffset: Bool, orientToPath: Bool, duration: TimeInterval) -> SKAction

Creates an action that moves the node along a path.

class func follow(CGPath, asOffset: Bool, orientToPath: Bool, speed: CGFloat) -> SKAction

Creates an action that moves the node at a specified speed along a path.

