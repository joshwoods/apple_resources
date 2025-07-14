

- SpriteKit
- SKAction
-  rotate(toAngle:duration:shortestUnitArc:) 

Type Method

# rotate(toAngle:duration:shortestUnitArc:)

Creates an action that rotates the node to an absolute value.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class func rotate(
    toAngle radians: CGFloat,
    duration: TimeInterval,
    shortestUnitArc: Bool
) -> SKAction
```

## Parameters 

`radians`  

The angle to rotate the node to, in radians.

`duration`  

The duration of the animation.

`shortestUnitArc`  

If true, the rotation is performed in whichever direction results in the smallest rotation. If false, the rotation is interpolated.

## Return Value

A new action object.

## Discussion

When the action executes, the node’s zRotation property is animated to the new angle.

This action is not reversible; the reverse of this action has the same duration but does not change anything.

## See Also

### Animating the Rotation of a Node

class func rotate(byAngle: CGFloat, duration: TimeInterval) -> SKAction

Creates an action that rotates the node by a relative value.

class func rotate(toAngle: CGFloat, duration: TimeInterval) -> SKAction

Creates an action that rotates the node counterclockwise to an absolute angle.

