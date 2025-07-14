

- Vision
-  VNDetectAnimalBodyPoseRequest 

Class

# VNDetectAnimalBodyPoseRequest

A request that detects an animal body pose.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
class VNDetectAnimalBodyPoseRequest
```

## Topics

### Determining Supported Joints

var supportedJointNames: [VNAnimalBodyPoseObservation.JointName]

Retrieves the joint names the request supports.

var supportedJointsGroupNames: [VNAnimalBodyPoseObservation.JointsGroupName]

Retrieves the joint group names the request supports.

### Accessing the Results

var results: [VNAnimalBodyPoseObservation]?

The animal body pose the request observes.

## Relationships

### Inherits From

- VNImageBasedRequest

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Animal body pose detection

Detecting animal body poses with Vision

Draw the skeleton of an animal by using Vision’s capability to detect animal body poses.

class VNAnimalBodyPoseObservation

An observation that provides the animal body points the analysis recognizes.

