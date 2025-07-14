

- Vision
- VNHumanBodyPoseObservation
-  VNHumanBodyPoseObservation.JointsGroupName 

Structure

# VNHumanBodyPoseObservation.JointsGroupName

The supported joint group names for the body pose.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
struct JointsGroupName
```

## Mentioned in 

Detecting Human Body Poses in Images

## Topics

### Head

static let face: VNHumanBodyPoseObservation.JointsGroupName

The face.

### Body

static let torso: VNHumanBodyPoseObservation.JointsGroupName

The torso.

### Arms

static let leftArm: VNHumanBodyPoseObservation.JointsGroupName

The left arm.

static let rightArm: VNHumanBodyPoseObservation.JointsGroupName

The right arm.

### Legs

static let leftLeg: VNHumanBodyPoseObservation.JointsGroupName

The left leg.

static let rightLeg: VNHumanBodyPoseObservation.JointsGroupName

The right leg.

### All

static let all: VNHumanBodyPoseObservation.JointsGroupName

All body point groups.

### Initializers

init(rawValue: VNRecognizedPointGroupKey)

Creates a joint group name with a recognized point group key.

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

struct JointName

The supported joint names for the body pose.

var availableJointsGroupNames: [VNHumanBodyPoseObservation.JointsGroupName]

The available joint group names in the observation.

func recognizedPoint(VNHumanBodyPoseObservation.JointName) throws -> VNRecognizedPoint

Retrieves the recognized point for a joint name.

func recognizedPoints(VNHumanBodyPoseObservation.JointsGroupName) throws -> [VNHumanBodyPoseObservation.JointName : VNRecognizedPoint]

Retrieves the recognized points associated with the joint group name.

