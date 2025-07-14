

- Vision
- VNAnimalBodyPoseObservation
-  recognizedPoints(\_:) 

Instance Method

# recognizedPoints(\_:)

Returns the points for a joint group name the observation recognizes.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
func recognizedPoints(_ jointsGroupName: VNAnimalBodyPoseObservation.JointsGroupName) throws -> [VNAnimalBodyPoseObservation.JointName : VNRecognizedPoint]
```

## Parameters 

`jointsGroupName`  

The joint group of the points to retrieve.

## Return Value

The dictionary of points the observation associates with the group name.

## See Also

### Accessing Points

var availableJointNames: [VNAnimalBodyPoseObservation.JointName]

The names of the available joints in the observation.

struct JointName

The joint names for an animal body pose.

var availableJointGroupNames: [VNAnimalBodyPoseObservation.JointsGroupName]

The available joint group names in the observation.

struct JointsGroupName

The joint group names for an animal body pose.

func recognizedPoint(VNAnimalBodyPoseObservation.JointName) throws -> VNRecognizedPoint

Returns the point for a joint name the observation recognizes.

