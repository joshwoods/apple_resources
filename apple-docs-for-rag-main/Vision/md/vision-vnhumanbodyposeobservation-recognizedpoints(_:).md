

- Vision
- VNHumanBodyPoseObservation
-  recognizedPoints(\_:) 

Instance Method

# recognizedPoints(\_:)

Retrieves the recognized points associated with the joint group name.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
func recognizedPoints(_ jointsGroupName: VNHumanBodyPoseObservation.JointsGroupName) throws -> [VNHumanBodyPoseObservation.JointName : VNRecognizedPoint]
```

## Parameters 

`jointsGroupName`  

The joint group name of the points to retrieve.

## Return Value

The array of points associated with the joint group name.

## Mentioned in 

Detecting Human Body Poses in Images

## See Also

### Accessing Points

var availableJointNames: [VNHumanBodyPoseObservation.JointName]

The names of the available joints in the observation.

struct JointName

The supported joint names for the body pose.

var availableJointsGroupNames: [VNHumanBodyPoseObservation.JointsGroupName]

The available joint group names in the observation.

struct JointsGroupName

The supported joint group names for the body pose.

func recognizedPoint(VNHumanBodyPoseObservation.JointName) throws -> VNRecognizedPoint

Retrieves the recognized point for a joint name.

