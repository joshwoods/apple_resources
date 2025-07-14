

- Vision
- VNHumanBodyPose3DObservation
-  VNHumanBodyPose3DObservation.JointsGroupName 

Structure

# VNHumanBodyPose3DObservation.JointsGroupName

The joint group names for a 3D body pose.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
struct JointsGroupName
```

## Topics

### Getting the Group Names

static let all: VNHumanBodyPose3DObservation.JointsGroupName

A group name that represents all joints.

static let head: VNHumanBodyPose3DObservation.JointsGroupName

A group name that represents the head joints.

static let leftArm: VNHumanBodyPose3DObservation.JointsGroupName

A group name that represents the left arm joints.

static let leftLeg: VNHumanBodyPose3DObservation.JointsGroupName

A group name that represents the left leg joints.

static let rightArm: VNHumanBodyPose3DObservation.JointsGroupName

A group name that represents the right arm joints.

static let rightLeg: VNHumanBodyPose3DObservation.JointsGroupName

A group name that represents the right leg joints.

static let torso: VNHumanBodyPose3DObservation.JointsGroupName

A group name that represents the torso joints.

### Creating a Group Name

init(rawValue: VNRecognizedPointGroupKey)

Creates a joint name with the key you specify.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### 3D body pose detection

Identifying 3D human body poses in images

Detect three-dimensional human body poses using the Vision framework.

Detecting human body poses in 3D with Vision

Render skeletons of 3D body pose points in a scene overlaying the input image.

class VNDetectHumanBodyPose3DRequest

A request that detects points on human bodies in 3D space, relative to the camera.

class VNHumanBodyPose3DObservation

An observation that provides the 3D body points the request recognizes.

class VNRecognizedPoints3DObservation

An observation that provides the 3D points for a request.

class VNHumanBodyRecognizedPoint3D

A recognized 3D point that includes a parent joint.

class VNPoint3D

An object that represents a 3D point in an image.

class VNRecognizedPoint3D

A 3D point that includes an identifier to the point.

struct JointName

The joint names for a 3D body pose.

