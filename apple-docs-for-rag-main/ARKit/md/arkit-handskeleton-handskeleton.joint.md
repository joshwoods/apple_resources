

- ARKit
- HandSkeleton
-  HandSkeleton.Joint 

Structure

# HandSkeleton.Joint

The name and position of an individual hand joint.

visionOS 1.0+

``` source
struct Joint
```

## Topics

### Inspecting hand joints

var name: HandSkeleton.JointName

A name that uniquely identifies this joint among others on the same skeleton.

var parentJoint: HandSkeleton.Joint?

The joint that’s connected to this joint and more closely connected to the base of the skeleton.

### Tracking the position of hand joints

var anchorFromJointTransform: simd_float4x4

The position and orientation of this joint relative to the base joint of the skeleton.

var parentFromJointTransform: simd_float4x4

The transform from the joint to its parent joint’s coordinate system.

var isTracked: Bool

A Boolean value that indicates whether ARKit is currently tracking this joint.

### Instance Properties

var description: String

A textual representation of this joint.

## Relationships

### Conforms To

- Copyable
- CustomStringConvertible
- Equatable
- Sendable

## See Also

### Retrieving specific hand joints

func joint(HandSkeleton.JointName) -> HandSkeleton.Joint

Retrieves a hand joint based on the joint name you specify.

enum JointName

The names of different hand joints.

