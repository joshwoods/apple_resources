

- Vision
-  VNHumanHandPoseObservation 

Class

# VNHumanHandPoseObservation

An observation that provides the hand points the analysis recognized.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
class VNHumanHandPoseObservation
```

## Topics

### Retrieving Points

var availableJointNames: [VNHumanHandPoseObservation.JointName]

The names of the available joints in the observation.

struct JointName

The supported joint names for the hand pose.

var availableJointsGroupNames: [VNHumanHandPoseObservation.JointsGroupName]

The joint group names available in the observation.

struct JointsGroupName

The supported joint group names for the hand pose.

func recognizedPoint(VNHumanHandPoseObservation.JointName) throws -> VNRecognizedPoint

Retrieves the recognized point for a joint name.

func recognizedPoints(VNHumanHandPoseObservation.JointsGroupName) throws -> [VNHumanHandPoseObservation.JointName : VNRecognizedPoint]

Retrieves the recognized points associated with the joint group name.

### Determining the Chirality

var chirality: VNChirality

The chirality, or handedness, of a pose.

enum VNChirality

Constants that the define the chirality, or handedness, of a pose.

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

class VNHumanBodyPoseObservation

An observation that provides the body points the analysis recognized.

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

