

- Vision
- VNHumanBodyPose3DObservation
-  availableJointsGroupNames 

Instance Property

# availableJointsGroupNames

The available joint group names in the observation.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
var availableJointsGroupNames: [VNHumanBodyPose3DObservation.JointsGroupName] { get }
```

## See Also

### Accessing Points

var availableJointNames: [VNHumanBodyPose3DObservation.JointName]

The names of the available joints in the observation.

struct JointName

The joint names for a 3D body pose.

struct JointsGroupName

The joint group names for a 3D body pose.

func recognizedPoint(VNHumanBodyPose3DObservation.JointName) throws -> VNHumanBodyRecognizedPoint3D

Returns the point for a joint name that the observation recognizes.

func recognizedPoints(VNHumanBodyPose3DObservation.JointsGroupName) throws -> [VNHumanBodyPose3DObservation.JointName : VNHumanBodyRecognizedPoint3D]

Returns a collection of points for the group name you specify.

