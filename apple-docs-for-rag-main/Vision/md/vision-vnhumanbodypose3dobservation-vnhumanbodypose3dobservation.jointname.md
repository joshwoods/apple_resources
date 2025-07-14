

- Vision
- VNHumanBodyPose3DObservation
-  VNHumanBodyPose3DObservation.JointName 

Structure

# VNHumanBodyPose3DObservation.JointName

The joint names for a 3D body pose.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
struct JointName
```

## Topics

### Getting the Head Joint Names

static let topHead: VNHumanBodyPose3DObservation.JointName

A joint name that represents the top of the head.

static let centerHead: VNHumanBodyPose3DObservation.JointName

A joint name that represents the center of the head.

### Getting the Arm Joint Names

static let centerShoulder: VNHumanBodyPose3DObservation.JointName

A joint name that represents the point between the shoulders.

static let leftShoulder: VNHumanBodyPose3DObservation.JointName

A joint name that represents the left shoulder.

static let rightShoulder: VNHumanBodyPose3DObservation.JointName

A joint name that represents the right shoulder.

static let leftElbow: VNHumanBodyPose3DObservation.JointName

A joint name that represents the left elbow.

static let rightElbow: VNHumanBodyPose3DObservation.JointName

A joint name that represents the right elbow.

static let leftWrist: VNHumanBodyPose3DObservation.JointName

A joint name that represents the left wrist.

static let rightWrist: VNHumanBodyPose3DObservation.JointName

A joint name that represents the right wrist.

### Getting the Leg Joint Names

static let leftHip: VNHumanBodyPose3DObservation.JointName

A joint name that represents the left hip.

static let rightHip: VNHumanBodyPose3DObservation.JointName

A joint name that represents the right hip.

static let leftKnee: VNHumanBodyPose3DObservation.JointName

A joint name that represents the left knee.

static let rightKnee: VNHumanBodyPose3DObservation.JointName

A joint name that represents the right knee.

static let leftAnkle: VNHumanBodyPose3DObservation.JointName

A joint name that represents the left ankle.

static let rightAnkle: VNHumanBodyPose3DObservation.JointName

A joint name that represents the right ankle.

### Getting the Root Joint Name

static let root: VNHumanBodyPose3DObservation.JointName

A joint name that represents the point between the left hip and right hip.

### Getting the Spine

static let spine: VNHumanBodyPose3DObservation.JointName

A joint name that represents the spine.

### Creating a Joint Name

init(rawValue: VNRecognizedPointKey)

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

struct JointsGroupName

The joint group names for a 3D body pose.

