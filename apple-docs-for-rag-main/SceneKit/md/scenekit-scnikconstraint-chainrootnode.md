

- SceneKit
- SCNIKConstraint
-  chainRootNode 

Instance Property

# chainRootNode

The parent node of the hierarchy affected by the constraint.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var chainRootNode: SCNNode { get }
```

## Discussion

The root node is the highest node in the hierarchy moved by the constraint. For example, a robot arm may have two arm segments and a hand connected to a body. The upper arm is a child node of the body, the lower arm is a child node of the upper arm, and the hand is a child node of the lower arm. In this case, the upper arm is the chain root node, because the body should not move to follow the hand.

## See Also

### Adjusting the Constraint’s Limits of Motion

func maxAllowedRotationAngle(forJoint: SCNNode) -> CGFloat

Returns the rotation limit, in degrees, for the specified node.

func setMaxAllowedRotationAngle(CGFloat, forJoint: SCNNode)

Sets the rotation limit, in degrees, for the specified node.

