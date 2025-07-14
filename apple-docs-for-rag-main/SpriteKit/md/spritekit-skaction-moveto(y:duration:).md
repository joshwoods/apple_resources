

- SpriteKit
- SKAction
-  moveTo(y:duration:) 

Type Method

# moveTo(y:duration:)

Creates an action that moves a node vertically.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class func moveTo(
    y: CGFloat,
    duration: TimeInterval
) -> SKAction
```

## Parameters 

`y`  

The y-value for the node’s new position.

`duration`  

The duration of the animation.

## Return Value

A new action object.

## Discussion

When the action executes, the node’s position property animates from its current position to its new position.

This action is not reversible; the reverse of this action has the same duration but does not move the node.

## See Also

### Animating a Node’s Position in a Linear Path

class func moveBy(x: CGFloat, y: CGFloat, duration: TimeInterval) -> SKAction

Creates an action that moves a node relative to its current position.

class func move(by: CGVector, duration: TimeInterval) -> SKAction

Creates an action that moves a node relative to its current position.

class func move(to: CGPoint, duration: TimeInterval) -> SKAction

Creates an action that moves a node to a new position.

class func moveTo(x: CGFloat, duration: TimeInterval) -> SKAction

Creates an action that moves a node horizontally.

