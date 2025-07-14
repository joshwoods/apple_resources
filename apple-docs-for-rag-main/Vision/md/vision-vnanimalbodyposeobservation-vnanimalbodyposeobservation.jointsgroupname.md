

- Vision
- VNAnimalBodyPoseObservation
-  VNAnimalBodyPoseObservation.JointsGroupName 

Structure

# VNAnimalBodyPoseObservation.JointsGroupName

The joint group names for an animal body pose.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
struct JointsGroupName
```

## Topics

### Getting the Group Names

static let all: VNAnimalBodyPoseObservation.JointsGroupName

A group name that represents all joints.

static let forelegs: VNAnimalBodyPoseObservation.JointsGroupName

A group name that represents the forelegs.

static let head: VNAnimalBodyPoseObservation.JointsGroupName

A group name that represents the head.

static let hindlegs: VNAnimalBodyPoseObservation.JointsGroupName

A group name that represents the hindlegs.

static let tail: VNAnimalBodyPoseObservation.JointsGroupName

A group name that represents the tail.

static let trunk: VNAnimalBodyPoseObservation.JointsGroupName

A group name that represents the trunk.

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

### Accessing Points

var availableJointNames: [VNAnimalBodyPoseObservation.JointName]

The names of the available joints in the observation.

struct JointName

The joint names for an animal body pose.

var availableJointGroupNames: [VNAnimalBodyPoseObservation.JointsGroupName]

The available joint group names in the observation.

func recognizedPoint(VNAnimalBodyPoseObservation.JointName) throws -> VNRecognizedPoint

Returns the point for a joint name the observation recognizes.

func recognizedPoints(VNAnimalBodyPoseObservation.JointsGroupName) throws -> [VNAnimalBodyPoseObservation.JointName : VNRecognizedPoint]

Returns the points for a joint group name the observation recognizes.

