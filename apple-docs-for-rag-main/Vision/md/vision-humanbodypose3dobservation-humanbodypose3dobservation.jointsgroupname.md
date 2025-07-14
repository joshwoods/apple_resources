

- Vision
- HumanBodyPose3DObservation
-  HumanBodyPose3DObservation.JointsGroupName 

Enumeration

# HumanBodyPose3DObservation.JointsGroupName

The supported joint group names for the body pose.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
enum JointsGroupName
```

## Topics

### Getting the group names

case head

case leftArm

case leftLeg

case rightArm

case rightLeg

case torso

## Relationships

### Conforms To

- CaseIterable
- Copyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Getting the joints

func allJoints(in: HumanBodyPose3DObservation.JointsGroupName?) -> [HumanBodyPose3DObservation.JointName : Joint3D]

Retrieves a dictionary of all joints in a joint group.

var availableJointsGroupNames: [HumanBodyPose3DObservation.JointsGroupName]

The names of the available joint groupings in the observation.

func joint(for: HumanBodyPose3DObservation.JointName) -> Joint3D?

Retrieves a joint for a given joint name.

var availableJointNames: [HumanBodyPose3DObservation.JointName]

The names of the available joints in the observation.

enum JointName

The supported joint names for the body pose.

