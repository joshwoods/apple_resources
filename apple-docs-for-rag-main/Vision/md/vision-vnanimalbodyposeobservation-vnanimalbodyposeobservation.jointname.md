

- Vision
- VNAnimalBodyPoseObservation
-  VNAnimalBodyPoseObservation.JointName 

Structure

# VNAnimalBodyPoseObservation.JointName

The joint names for an animal body pose.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
struct JointName
```

## Topics

### Getting the Head Joint Names

static let leftEarTop: VNAnimalBodyPoseObservation.JointName

A joint name that represents the top of the left ear.

static let leftEarMiddle: VNAnimalBodyPoseObservation.JointName

A joint name that represents the middle of the left ear.

static let leftEarBottom: VNAnimalBodyPoseObservation.JointName

A joint name that represents the bottom of the left ear.

static let leftEye: VNAnimalBodyPoseObservation.JointName

A joint name that represents the left eye.

static let neck: VNAnimalBodyPoseObservation.JointName

A joint name that represents the neck.

static let nose: VNAnimalBodyPoseObservation.JointName

A joint name that represents the nose.

static let rightEye: VNAnimalBodyPoseObservation.JointName

A joint name that represents the right eye.

static let rightEarTop: VNAnimalBodyPoseObservation.JointName

A joint name that represents the top of the right ear.

static let rightEarMiddle: VNAnimalBodyPoseObservation.JointName

A joint name that represents the middle of the right ear.

static let rightEarBottom: VNAnimalBodyPoseObservation.JointName

A joint name that represents the bottom of the right ear.

### Getting the Leg Joint Names

static let leftBackElbow: VNAnimalBodyPoseObservation.JointName

A joint name that represents the back of the left elbow.

static let leftFrontElbow: VNAnimalBodyPoseObservation.JointName

A joint name that represents the front of the left elbow.

static let rightFrontElbow: VNAnimalBodyPoseObservation.JointName

A joint name that represents the front of the right elbow.

static let rightBackElbow: VNAnimalBodyPoseObservation.JointName

A joint name that represents the back of the right elbow.

static let leftBackKnee: VNAnimalBodyPoseObservation.JointName

A joint name that represents the back of the left knee.

static let leftFrontKnee: VNAnimalBodyPoseObservation.JointName

A joint name that represents the front of the left knee.

static let rightBackKnee: VNAnimalBodyPoseObservation.JointName

A joint name that represents the back of the right knee.

static let rightFrontKnee: VNAnimalBodyPoseObservation.JointName

A joint name that represents the front of the right knee.

static let leftBackPaw: VNAnimalBodyPoseObservation.JointName

A joint name that represents the back of the left paw.

static let leftFrontPaw: VNAnimalBodyPoseObservation.JointName

A joint name that represents the front of the left paw.

static let rightBackPaw: VNAnimalBodyPoseObservation.JointName

A joint name that represents the back of the right paw.

static let rightFrontPaw: VNAnimalBodyPoseObservation.JointName

A joint name that represents the front of the right paw.

### Getting the Tail Joint Names

static let tailTop: VNAnimalBodyPoseObservation.JointName

A joint name that represents the top of the tail.

static let tailMiddle: VNAnimalBodyPoseObservation.JointName

A joint name that represents the middle of the tail.

static let tailBottom: VNAnimalBodyPoseObservation.JointName

A joint name that represents the bottom of the tail.

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

### Accessing Points

var availableJointNames: [VNAnimalBodyPoseObservation.JointName]

The names of the available joints in the observation.

var availableJointGroupNames: [VNAnimalBodyPoseObservation.JointsGroupName]

The available joint group names in the observation.

struct JointsGroupName

The joint group names for an animal body pose.

func recognizedPoint(VNAnimalBodyPoseObservation.JointName) throws -> VNRecognizedPoint

Returns the point for a joint name the observation recognizes.

func recognizedPoints(VNAnimalBodyPoseObservation.JointsGroupName) throws -> [VNAnimalBodyPoseObservation.JointName : VNRecognizedPoint]

Returns the points for a joint group name the observation recognizes.

