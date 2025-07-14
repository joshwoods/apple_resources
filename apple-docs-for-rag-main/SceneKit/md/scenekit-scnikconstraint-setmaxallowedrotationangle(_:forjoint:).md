

- SceneKit
- SCNIKConstraint
-  setMaxAllowedRotationAngle(\_:forJoint:) 

Instance Method

# setMaxAllowedRotationAngle(\_:forJoint:)

Sets the rotation limit, in degrees, for the specified node.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
func setMaxAllowedRotationAngle(
    _ angle: CGFloat,
    forJoint node: SCNNode
)
```

## Parameters 

`angle`  

The maximum rotation, in degrees, that SceneKit should apply to the specified node when evaluating the constraint.

`node`  

A node affected by the constraint—either the node whose constraints property references the constraint, or one of that node’s parent or ancestor nodes up to the node specified by the constraint’s chainRootNode property.

## Discussion

When SceneKit evaluates the IK constraint, it checks the target orientations of each node in the chain relative to their initial orientations (as of when the constraint was applied to a node). For each node in the chain, SceneKit limits the rotation (in any direction) between the initial and target orientations to the `angle` value specified with this method.

The default rotation limit for each joint is 180 degrees in either direction, allowing unconstrained rotation.

## See Also

### Adjusting the Constraint’s Limits of Motion

var chainRootNode: SCNNode

The parent node of the hierarchy affected by the constraint.

func maxAllowedRotationAngle(forJoint: SCNNode) -> CGFloat

Returns the rotation limit, in degrees, for the specified node.

