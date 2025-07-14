

- Vision
- VNHumanBodyPose3DObservation
-  recognizedPoints(\_:) 

Instance Method

# recognizedPoints(\_:)

Returns a collection of points for the group name you specify.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
func recognizedPoints(_ jointsGroupName: VNHumanBodyPose3DObservation.JointsGroupName) throws -> [VNHumanBodyPose3DObservation.JointName : VNHumanBodyRecognizedPoint3D]
```

## Parameters 

`jointsGroupName`  

The name of the human body joints group.

## Return Value

A collection of points.

## See Also

### Accessing Points

var availableJointNames: [VNHumanBodyPose3DObservation.JointName]

The names of the available joints in the observation.

struct JointName

The joint names for a 3D body pose.

var availableJointsGroupNames: [VNHumanBodyPose3DObservation.JointsGroupName]

The available joint group names in the observation.

struct JointsGroupName

The joint group names for a 3D body pose.

func recognizedPoint(VNHumanBodyPose3DObservation.JointName) throws -> VNHumanBodyRecognizedPoint3D

Returns the point for a joint name that the observation recognizes.

