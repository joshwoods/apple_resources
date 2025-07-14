

- Vision
- VNHumanHandPoseObservation
-  VNHumanHandPoseObservation.JointsGroupName 

Structure

# VNHumanHandPoseObservation.JointsGroupName

The supported joint group names for the hand pose.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
struct JointsGroupName
```

## Topics

### Group Names

static let thumb: VNHumanHandPoseObservation.JointsGroupName

The thumb.

static let indexFinger: VNHumanHandPoseObservation.JointsGroupName

The index finger.

static let littleFinger: VNHumanHandPoseObservation.JointsGroupName

The little finger.

static let middleFinger: VNHumanHandPoseObservation.JointsGroupName

The middle finger.

static let ringFinger: VNHumanHandPoseObservation.JointsGroupName

The ring finger.

static let all: VNHumanHandPoseObservation.JointsGroupName

All hand group names.

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

### Retrieving Points

var availableJointNames: [VNHumanHandPoseObservation.JointName]

The names of the available joints in the observation.

struct JointName

The supported joint names for the hand pose.

var availableJointsGroupNames: [VNHumanHandPoseObservation.JointsGroupName]

The joint group names available in the observation.

func recognizedPoint(VNHumanHandPoseObservation.JointName) throws -> VNRecognizedPoint

Retrieves the recognized point for a joint name.

func recognizedPoints(VNHumanHandPoseObservation.JointsGroupName) throws -> [VNHumanHandPoseObservation.JointName : VNRecognizedPoint]

Retrieves the recognized points associated with the joint group name.

