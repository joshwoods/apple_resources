

- Vision
- VNHumanBodyPoseObservation
-  VNHumanBodyPoseObservation.JointName 

Structure

# VNHumanBodyPoseObservation.JointName

The supported joint names for the body pose.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
struct JointName
```

## Topics

### Head

static let leftEar: VNHumanBodyPoseObservation.JointName

The left ear.

static let leftEye: VNHumanBodyPoseObservation.JointName

The left eye.

static let rightEar: VNHumanBodyPoseObservation.JointName

The right ear.

static let rightEye: VNHumanBodyPoseObservation.JointName

The right eye.

static let neck: VNHumanBodyPoseObservation.JointName

The neck.

static let nose: VNHumanBodyPoseObservation.JointName

The nose.

### Arms

static let leftShoulder: VNHumanBodyPoseObservation.JointName

The left shoulder.

static let leftElbow: VNHumanBodyPoseObservation.JointName

The left elbow.

static let leftWrist: VNHumanBodyPoseObservation.JointName

The left wrist.

static let rightShoulder: VNHumanBodyPoseObservation.JointName

The right shoulder.

static let rightElbow: VNHumanBodyPoseObservation.JointName

The right elbow.

static let rightWrist: VNHumanBodyPoseObservation.JointName

The right wrist.

### Waist

static let root: VNHumanBodyPoseObservation.JointName

The root (waist).

### Legs

static let leftHip: VNHumanBodyPoseObservation.JointName

The left hip.

static let leftKnee: VNHumanBodyPoseObservation.JointName

The left knee.

static let leftAnkle: VNHumanBodyPoseObservation.JointName

The left ankle.

static let rightHip: VNHumanBodyPoseObservation.JointName

The right hip.

static let rightKnee: VNHumanBodyPoseObservation.JointName

The right knee.

static let rightAnkle: VNHumanBodyPoseObservation.JointName

The right ankle.

### Initializers

init(rawValue: VNRecognizedPointKey)

Creates a joint name with a recognized point key.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Accessing Points

var availableJointNames: [VNHumanBodyPoseObservation.JointName]

The names of the available joints in the observation.

var availableJointsGroupNames: [VNHumanBodyPoseObservation.JointsGroupName]

The available joint group names in the observation.

struct JointsGroupName

The supported joint group names for the body pose.

func recognizedPoint(VNHumanBodyPoseObservation.JointName) throws -> VNRecognizedPoint

Retrieves the recognized point for a joint name.

func recognizedPoints(VNHumanBodyPoseObservation.JointsGroupName) throws -> [VNHumanBodyPoseObservation.JointName : VNRecognizedPoint]

Retrieves the recognized points associated with the joint group name.

