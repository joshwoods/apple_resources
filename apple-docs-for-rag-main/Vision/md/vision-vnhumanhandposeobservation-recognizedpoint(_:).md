

- Vision
- VNHumanHandPoseObservation
-  recognizedPoint(\_:) 

Instance Method

# recognizedPoint(\_:)

Retrieves the recognized point for a joint name.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
func recognizedPoint(_ jointName: VNHumanHandPoseObservation.JointName) throws -> VNRecognizedPoint
```

## Parameters 

`jointName`  

The joint name of the point to retrieve.

## Return Value

The point for the joint name.

## See Also

### Retrieving Points

var availableJointNames: [VNHumanHandPoseObservation.JointName]

The names of the available joints in the observation.

struct JointName

The supported joint names for the hand pose.

var availableJointsGroupNames: [VNHumanHandPoseObservation.JointsGroupName]

The joint group names available in the observation.

struct JointsGroupName

The supported joint group names for the hand pose.

func recognizedPoints(VNHumanHandPoseObservation.JointsGroupName) throws -> [VNHumanHandPoseObservation.JointName : VNRecognizedPoint]

Retrieves the recognized points associated with the joint group name.

