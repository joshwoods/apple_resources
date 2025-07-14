

- SceneKit
- SCNAction
-  rotateTo(x:y:z:duration:usesShortestUnitArc:) 

Type Method

# rotateTo(x:y:z:duration:usesShortestUnitArc:)

Creates an action that rotates the node to absolute angles in each of the three principal axes.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
class func rotateTo(
    x xAngle: CGFloat,
    y yAngle: CGFloat,
    z zAngle: CGFloat,
    duration: TimeInterval,
    usesShortestUnitArc shortestUnitArc: Bool
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

`shortestUnitArc`  

If false (the default), the animation interpolates each component of the node’s rotation between its current value and the new value. If true, the animation makes the most direct rotation possible from the node’s current orientation to the new orientation.

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

class func rotate(by: CGFloat, around: SCNVector3, duration: TimeInterval) -> SCNAction

Creates an action that rotates the node by an angle around a specified axis.

class func rotate(toAxisAngle: SCNVector4, duration: TimeInterval) -> SCNAction

Creates an action that rotates the node to an absolute angle around a specified axis.

