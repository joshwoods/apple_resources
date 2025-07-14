

- SceneKit
- SCNAction
-  rotate(toAxisAngle:duration:) 

Type Method

# rotate(toAxisAngle:duration:)

Creates an action that rotates the node to an absolute angle around a specified axis.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
class func rotate(
    toAxisAngle axisAngle: SCNVector4,
    duration: TimeInterval
) -> SCNAction
```

## Parameters 

`axisAngle`  

A four-component vector whose first three components are a vector in the node’s local coordinate space specifying an axis and whose fourth component is the amount to rotate the node counterclockwise around that axis, in radians.

`duration`  

The duration, in seconds, of the animation.

## Return Value

A new action object.

## Discussion

When the action executes, the node’s rotation property animates to the new angle.

This action is not reversible; the reverse of this action has the same duration but does not change anything.

## See Also

### Creating Actions That Rotate a Node

class func rotateBy(x: CGFloat, y: CGFloat, z: CGFloat, duration: TimeInterval) -> SCNAction

Creates an action that rotates the node in each of the three principal axes by angles relative to its current orientation.

class func rotateTo(x: CGFloat, y: CGFloat, z: CGFloat, duration: TimeInterval) -> SCNAction

Creates an action that rotates the node to absolute angles in each of the three principal axes.

class func rotateTo(x: CGFloat, y: CGFloat, z: CGFloat, duration: TimeInterval, usesShortestUnitArc: Bool) -> SCNAction

Creates an action that rotates the node to absolute angles in each of the three principal axes.

class func rotate(by: CGFloat, around: SCNVector3, duration: TimeInterval) -> SCNAction

Creates an action that rotates the node by an angle around a specified axis.

