

- SpriteKit
- SKAction
-  move(by:duration:) 

Type Method

# move(by:duration:)

Creates an action that moves a node relative to its current position.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class func move(
    by delta: CGVector,
    duration: TimeInterval
) -> SKAction
```

## Parameters 

`delta`  

A vector that describes the change to apply to the node’s position.

`duration`  

The duration of the animation.

## Return Value

A new action object.

## Discussion

When the action executes, the node’s position property animates from its current position to its new position.

This action is reversible; the reverse is created as if the following code is executed:

- Swift
- Obj-C

```
let negDelta = CGVector(dx: -deltaX, dy: -deltaY)
let action = SKAction.move(by: negDelta, duration: sec)
```

```
CGVector negDelta = CGVectorMake(-delta.dx,-delta.dy);
[SKAction moveBy: negDelta duration: sec];
```

## See Also

### Animating a Node’s Position in a Linear Path

class func moveBy(x: CGFloat, y: CGFloat, duration: TimeInterval) -> SKAction

Creates an action that moves a node relative to its current position.

class func move(to: CGPoint, duration: TimeInterval) -> SKAction

Creates an action that moves a node to a new position.

class func moveTo(x: CGFloat, duration: TimeInterval) -> SKAction

Creates an action that moves a node horizontally.

class func moveTo(y: CGFloat, duration: TimeInterval) -> SKAction

Creates an action that moves a node vertically.

