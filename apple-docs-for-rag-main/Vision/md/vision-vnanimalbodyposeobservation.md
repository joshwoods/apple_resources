

- Vision
-  VNAnimalBodyPoseObservation 

Class

# VNAnimalBodyPoseObservation

An observation that provides the animal body points the analysis recognizes.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
class VNAnimalBodyPoseObservation
```

## Topics

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

func recognizedPoints(VNAnimalBodyPoseObservation.JointsGroupName) throws -> [VNAnimalBodyPoseObservation.JointName : VNRecognizedPoint]

Returns the points for a joint group name the observation recognizes.

## Relationships

### Inherits From

- VNRecognizedPointsObservation

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding
- VNRequestRevisionProviding

## See Also

### Animal body pose detection

Detecting animal body poses with Vision

Draw the skeleton of an animal by using Vision’s capability to detect animal body poses.

class VNDetectAnimalBodyPoseRequest

A request that detects an animal body pose.

