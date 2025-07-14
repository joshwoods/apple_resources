

- SceneKit
- SCNAction
-  rotate(by:around:duration:) 

Type Method

# rotate(by:around:duration:)

Creates an action that rotates the node by an angle around a specified axis.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
class func rotate(
    by angle: CGFloat,
    around axis: SCNVector3,
    duration: TimeInterval
) -> SCNAction
```

## Parameters 

`angle`  

The amount to rotate the node counterclockwise around the specified axis, in radians.

`axis`  

A vector in the node’s local coordinate space whose direction specifies the axis of rotation.

`duration`  

The duration, in seconds, of the animation.

## Return Value

A new action object.

## Discussion

When the action executes, the node’s rotation property animates to the new angle.

This action is reversible; the reverse is created as if the following code had been executed:

```
[SCNAction rotateByAngle: -angle aroundAxis: axis duration: sec];
```

## See Also

### Creating Actions That Rotate a Node

class func rotateBy(x: CGFloat, y: CGFloat, z: CGFloat, duration: TimeInterval) -> SCNAction

Creates an action that rotates the node in each of the three principal axes by angles relative to its current orientation.

class func rotateTo(x: CGFloat, y: CGFloat, z: CGFloat, duration: TimeInterval) -> SCNAction

Creates an action that rotates the node to absolute angles in each of the three principal axes.

class func rotateTo(x: CGFloat, y: CGFloat, z: CGFloat, duration: TimeInterval, usesShortestUnitArc: Bool) -> SCNAction

Creates an action that rotates the node to absolute angles in each of the three principal axes.

class func rotate(toAxisAngle: SCNVector4, duration: TimeInterval) -> SCNAction

Creates an action that rotates the node to an absolute angle around a specified axis.

