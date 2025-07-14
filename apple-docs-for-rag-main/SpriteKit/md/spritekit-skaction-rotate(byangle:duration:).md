

- SpriteKit
- SKAction
-  rotate(byAngle:duration:) 

Type Method

# rotate(byAngle:duration:)

Creates an action that rotates the node by a relative value.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class func rotate(
    byAngle radians: CGFloat,
    duration: TimeInterval
) -> SKAction
```

## Parameters 

`radians`  

The amount to rotate the node, in radians.

`duration`  

The duration of the animation.

## Return Value

A new action object.

## Discussion

When the action executes, the node’s zRotation property animates to the new angle.

This action is reversible; the reverse is created as if the following code is executed:

- Swift
- Obj-C

```
let action = SKAction.rotate(byAngle: -radians, duration: sec)
```

```
[SKAction rotateByAngle: -radians duration: sec];
```

## See Also

### Animating the Rotation of a Node

class func rotate(toAngle: CGFloat, duration: TimeInterval) -> SKAction

Creates an action that rotates the node counterclockwise to an absolute angle.

class func rotate(toAngle: CGFloat, duration: TimeInterval, shortestUnitArc: Bool) -> SKAction

Creates an action that rotates the node to an absolute value.

