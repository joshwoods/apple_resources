

- Vision
- VNAnimalBodyPoseObservation
-  recognizedPoint(\_:) 

Instance Method

# recognizedPoint(\_:)

Returns the point for a joint name the observation recognizes.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
func recognizedPoint(_ jointName: VNAnimalBodyPoseObservation.JointName) throws -> VNRecognizedPoint
```

## Parameters 

`jointName`  

The joint name to retrieve.

## Return Value

The point for the joint name.

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

func recognizedPoints(VNAnimalBodyPoseObservation.JointsGroupName) throws -> [VNAnimalBodyPoseObservation.JointName : VNRecognizedPoint]

Returns the points for a joint group name the observation recognizes.

