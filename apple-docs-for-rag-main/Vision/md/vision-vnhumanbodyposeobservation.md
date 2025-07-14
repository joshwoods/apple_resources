

- Vision
-  VNHumanBodyPoseObservation 

Class

# VNHumanBodyPoseObservation

An observation that provides the body points the analysis recognized.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
class VNHumanBodyPoseObservation
```

## Mentioned in 

Detecting Human Body Poses in Images

## Topics

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

func recognizedPoints(VNHumanBodyPoseObservation.JointsGroupName) throws -> [VNHumanBodyPoseObservation.JointName : VNRecognizedPoint]

Retrieves the recognized points associated with the joint group name.

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

### Body and hand pose detection

Detecting Human Body Poses in Images

Add the capability to detect human body poses to your app using the Vision framework.

Detecting Hand Poses with Vision

Create a virtual drawing app by using Vision’s capability to detect hand poses.

class VNDetectHumanBodyPoseRequest

A request that detects a human body pose.

class VNDetectHumanHandPoseRequest

A request that detects a human hand pose.

class VNRecognizedPointsObservation

An observation that provides the points the analysis recognized.

class VNHumanHandPoseObservation

An observation that provides the hand points the analysis recognized.

class VNPoint

An immutable object that represents a single 2D point in an image.

class VNDetectedPoint

An object that represents a normalized point in an image, along with a confidence value.

class VNRecognizedPoint

An object that represents a normalized point in an image, along with an identifier label and a confidence value.

struct VNRecognizedPointKey

The data type for all recognized point keys.

struct VNRecognizedPointGroupKey

The data type for all recognized-point group keys.

