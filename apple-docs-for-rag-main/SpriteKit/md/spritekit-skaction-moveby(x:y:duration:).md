

- SpriteKit
- SKAction
-  moveBy(x:y:duration:) 

Type Method

# moveBy(x:y:duration:)

Creates an action that moves a node relative to its current position.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class func moveBy(
    x deltaX: CGFloat,
    y deltaY: CGFloat,
    duration: TimeInterval
) -> SKAction
```

## Parameters 

`deltaX`  

The x-value, in points, to add to the node’s position.

`deltaY`  

The y-value, in points, to add to the node’s position.

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
let action = SKAction.moveBy(x: -deltaX, y: -deltaX, duration: sec)
```

```
[SKAction moveByX: -deltaX y: -deltaY duration: sec];
```

## See Also

### Animating a Node’s Position in a Linear Path

class func move(by: CGVector, duration: TimeInterval) -> SKAction

Creates an action that moves a node relative to its current position.

class func move(to: CGPoint, duration: TimeInterval) -> SKAction

Creates an action that moves a node to a new position.

class func moveTo(x: CGFloat, duration: TimeInterval) -> SKAction

Creates an action that moves a node horizontally.

class func moveTo(y: CGFloat, duration: TimeInterval) -> SKAction

Creates an action that moves a node vertically.

