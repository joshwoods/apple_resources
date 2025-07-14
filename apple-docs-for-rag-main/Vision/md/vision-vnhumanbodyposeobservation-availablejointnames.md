

- Vision
- VNHumanBodyPoseObservation
-  availableJointNames 

Instance Property

# availableJointNames

The names of the available joints in the observation.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
var availableJointNames: [VNHumanBodyPoseObservation.JointName] { get }
```

## See Also

### Accessing Points

struct JointName

The supported joint names for the body pose.

var availableJointsGroupNames: [VNHumanBodyPoseObservation.JointsGroupName]

The available joint group names in the observation.

struct JointsGroupName

The supported joint group names for the body pose.

func recognizedPoint(VNHumanBodyPoseObservation.JointName) throws -> VNRecognizedPoint

Retrieves the recognized point for a joint name.

func recognizedPoints(VNHumanBodyPoseObservation.JointsGroupName) throws -> [VNHumanBodyPoseObservation.JointName : VNRecognizedPoint]

Retrieves the recognized points associated with the joint group name.

