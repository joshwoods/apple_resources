

- Vision
- VNAnimalBodyPoseObservation
-  availableJointGroupNames 

Instance Property

# availableJointGroupNames

The available joint group names in the observation.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
var availableJointGroupNames: [VNAnimalBodyPoseObservation.JointsGroupName] { get }
```

## See Also

### Accessing Points

var availableJointNames: [VNAnimalBodyPoseObservation.JointName]

The names of the available joints in the observation.

struct JointName

The joint names for an animal body pose.

struct JointsGroupName

The joint group names for an animal body pose.

func recognizedPoint(VNAnimalBodyPoseObservation.JointName) throws -> VNRecognizedPoint

Returns the point for a joint name the observation recognizes.

func recognizedPoints(VNAnimalBodyPoseObservation.JointsGroupName) throws -> [VNAnimalBodyPoseObservation.JointName : VNRecognizedPoint]

Returns the points for a joint group name the observation recognizes.

