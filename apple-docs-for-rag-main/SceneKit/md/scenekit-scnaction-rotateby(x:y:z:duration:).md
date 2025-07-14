

- SceneKit
- SCNAction
-  rotateBy(x:y:z:duration:) 

Type Method

# rotateBy(x:y:z:duration:)

Creates an action that rotates the node in each of the three principal axes by angles relative to its current orientation.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
class func rotateBy(
    x xAngle: CGFloat,
    y yAngle: CGFloat,
    z zAngle: CGFloat,
    duration: TimeInterval
) -> SCNAction
```

## Parameters 

`xAngle`  

The amount to rotate the node counterclockwise around the x-axis of its local coordinate space, in radians.

`yAngle`  

The amount to rotate the node counterclockwise around the y-axis of its local coordinate space, in radians.

`zAngle`  

The amount to rotate the node counterclockwise around the z-axis of its local coordinate space, in radians.

`duration`  

The duration, in seconds, of the animation.

## Return Value

A new action object.

## Discussion

When the action executes, the node’s rotation property animates to the new angle.

This action is reversible; the reverse is created as if the following code had been executed:

```
[SCNAction rotateByX: -xAngle y: -yAngle z: -zAngle duration: duration];
```

## See Also

### Creating Actions That Rotate a Node

class func rotateTo(x: CGFloat, y: CGFloat, z: CGFloat, duration: TimeInterval) -> SCNAction

Creates an action that rotates the node to absolute angles in each of the three principal axes.

class func rotateTo(x: CGFloat, y: CGFloat, z: CGFloat, duration: TimeInterval, usesShortestUnitArc: Bool) -> SCNAction

Creates an action that rotates the node to absolute angles in each of the three principal axes.

class func rotate(by: CGFloat, around: SCNVector3, duration: TimeInterval) -> SCNAction

Creates an action that rotates the node by an angle around a specified axis.

class func rotate(toAxisAngle: SCNVector4, duration: TimeInterval) -> SCNAction

Creates an action that rotates the node to an absolute angle around a specified axis.

