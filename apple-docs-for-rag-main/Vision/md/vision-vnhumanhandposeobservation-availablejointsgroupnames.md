

- Vision
- VNHumanHandPoseObservation
-  availableJointsGroupNames 

Instance Property

# availableJointsGroupNames

The joint group names available in the observation.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
var availableJointsGroupNames: [VNHumanHandPoseObservation.JointsGroupName] { get }
```

## See Also

### Retrieving Points

var availableJointNames: [VNHumanHandPoseObservation.JointName]

The names of the available joints in the observation.

struct JointName

The supported joint names for the hand pose.

struct JointsGroupName

The supported joint group names for the hand pose.

func recognizedPoint(VNHumanHandPoseObservation.JointName) throws -> VNRecognizedPoint

Retrieves the recognized point for a joint name.

func recognizedPoints(VNHumanHandPoseObservation.JointsGroupName) throws -> [VNHumanHandPoseObservation.JointName : VNRecognizedPoint]

Retrieves the recognized points associated with the joint group name.

