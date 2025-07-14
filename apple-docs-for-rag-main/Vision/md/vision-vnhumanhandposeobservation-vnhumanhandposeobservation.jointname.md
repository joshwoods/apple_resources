

- Vision
- VNHumanHandPoseObservation
-  VNHumanHandPoseObservation.JointName 

Structure

# VNHumanHandPoseObservation.JointName

The supported joint names for the hand pose.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
struct JointName
```

## Topics

### Thumb

static let thumbTip: VNHumanHandPoseObservation.JointName

The tip of the thumb.

static let thumbIP: VNHumanHandPoseObservation.JointName

The thumb’s interphalangeal (IP) joint.

static let thumbMP: VNHumanHandPoseObservation.JointName

The thumb’s metacarpophalangeal (MP) joint.

static let thumbCMC: VNHumanHandPoseObservation.JointName

The thumb’s carpometacarpal (CMC) joint.

### Index

static let indexTip: VNHumanHandPoseObservation.JointName

The tip of the index finger.

static let indexDIP: VNHumanHandPoseObservation.JointName

The index finger’s distal interphalangeal (DIP) joint.

static let indexPIP: VNHumanHandPoseObservation.JointName

The index finger’s proximal interphalangeal (PIP) joint.

static let indexMCP: VNHumanHandPoseObservation.JointName

The index finger’s metacarpophalangeal (MCP) joint.

### Middle

static let middleTip: VNHumanHandPoseObservation.JointName

The tip of the middle finger.

static let middleDIP: VNHumanHandPoseObservation.JointName

The middle finger’s distal interphalangeal (DIP) joint.

static let middlePIP: VNHumanHandPoseObservation.JointName

The middle finger’s proximal interphalangeal (PIP) joint.

static let middleMCP: VNHumanHandPoseObservation.JointName

The middle finger’s metacarpophalangeal (MCP) joint.

### Ring

static let ringTip: VNHumanHandPoseObservation.JointName

The tip of the ring finger.

static let ringDIP: VNHumanHandPoseObservation.JointName

The ring finger’s distal interphalangeal (DIP) joint.

static let ringPIP: VNHumanHandPoseObservation.JointName

The ring finger’s proximal interphalangeal (PIP) joint.

static let ringMCP: VNHumanHandPoseObservation.JointName

The ring finger’s metacarpophalangeal (MCP) joint.

### Little

static let littleTip: VNHumanHandPoseObservation.JointName

The tip of the little finger.

static let littleDIP: VNHumanHandPoseObservation.JointName

The little finger’s distal interphalangeal (DIP) joint.

static let littlePIP: VNHumanHandPoseObservation.JointName

The little finger’s proximal interphalangeal (PIP) joint.

static let littleMCP: VNHumanHandPoseObservation.JointName

The little finger’s metacarpophalangeal (MCP) joint.

### Wrist

static let wrist: VNHumanHandPoseObservation.JointName

The wrist.

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

### Retrieving Points

var availableJointNames: [VNHumanHandPoseObservation.JointName]

The names of the available joints in the observation.

var availableJointsGroupNames: [VNHumanHandPoseObservation.JointsGroupName]

The joint group names available in the observation.

struct JointsGroupName

The supported joint group names for the hand pose.

func recognizedPoint(VNHumanHandPoseObservation.JointName) throws -> VNRecognizedPoint

Retrieves the recognized point for a joint name.

func recognizedPoints(VNHumanHandPoseObservation.JointsGroupName) throws -> [VNHumanHandPoseObservation.JointName : VNRecognizedPoint]

Retrieves the recognized points associated with the joint group name.

