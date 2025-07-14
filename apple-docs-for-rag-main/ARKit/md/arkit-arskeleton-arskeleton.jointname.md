

- ARKit
- ARSkeleton
-  ARSkeleton.JointName 

Structure

# ARSkeleton.JointName

A name identifier for a joint.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
struct JointName
```

## Discussion

Use this class to access information about a named joint, such as its index in a skeleton’s array of joints, or its position on the screen or in the physical environment.

When you’re tracking a body in 2D space, you get the screen-space position of a named joint by using the landmark(for:) function.

When you’re tracking a body in 3D space, you get a named joint’s position in either local or model space by using the localTransform(for:) or modelTransform(for:) functions, respectively.

## Topics

### Creating a Joint Name

init(rawValue: String)

Creates a new joint name.

init?(VNRecognizedPointKey)

Returns a joint name that corresponds to a key point defined in a human body pose.

struct VNRecognizedPointKey

The data type for all recognized point keys.

### Identifying Joints

static let root: ARSkeleton.JointName

A skeletal joint that’s the root of all other joints.

static let head: ARSkeleton.JointName

A skeletal joint that ARKit tracks representing the head.

static let leftFoot: ARSkeleton.JointName

A skeletal joint that ARKit tracks representing the left foot.

static let leftHand: ARSkeleton.JointName

A skeletal joint that ARKit tracks representing the left hand.

static let leftShoulder: ARSkeleton.JointName

A skeletal joint that ARKit tracks representing the left shoulder.

static let rightFoot: ARSkeleton.JointName

A skeletal joint that ARKit tracks representing the right foot.

static let rightHand: ARSkeleton.JointName

A skeletal joint that ARKit tracks representing the right hand.

static let rightShoulder: ARSkeleton.JointName

A skeletal joint that ARKit tracks representing the right shoulder.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Getting Joint Information

var definition: ARSkeletonDefinition

The particular configuration of joints that define a body’s current state.

func isJointTracked(Int) -> Bool

Tells you whether ARKit tracks a joint at a particular index.

