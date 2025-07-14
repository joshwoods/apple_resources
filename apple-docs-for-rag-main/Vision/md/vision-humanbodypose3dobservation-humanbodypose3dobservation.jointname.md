

- Vision
- HumanBodyPose3DObservation
-  HumanBodyPose3DObservation.JointName 

Enumeration

# HumanBodyPose3DObservation.JointName

The supported joint names for the body pose.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
enum JointName
```

## Topics

### Getting the joint names

case centerHead

case centerShoulder

case leftAnkle

case leftElbow

case leftHip

case leftKnee

case leftShoulder

case leftWrist

case rightAnkle

case rightElbow

case rightHip

case rightKnee

case rightShoulder

case rightWrist

case root

case spine

case topHead

## Relationships

### Conforms To

- Copyable
- Decodable
- Encodable
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

enum JointsGroupName

The supported joint group names for the body pose.

func joint(for: HumanBodyPose3DObservation.JointName) -> Joint3D?

Retrieves a joint for a given joint name.

var availableJointNames: [HumanBodyPose3DObservation.JointName]

The names of the available joints in the observation.

