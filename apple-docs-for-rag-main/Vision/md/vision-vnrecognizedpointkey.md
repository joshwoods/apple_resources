

- Vision
-  VNRecognizedPointKey 

Structure

# VNRecognizedPointKey

The data type for all recognized point keys.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.0+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
struct VNRecognizedPointKey
```

## Topics

### Landmarks

Body Landmarks

The body landmarks that Vision detects.

Hand Landmarks

The hand landmarks that Vision detects.

### Initializers

init(rawValue: String)

Creates a recognized point key with a string value.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

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

class VNHumanHandPoseObservation

An observation that provides the hand points the analysis recognized.

class VNPoint

An immutable object that represents a single 2D point in an image.

class VNDetectedPoint

An object that represents a normalized point in an image, along with a confidence value.

class VNRecognizedPoint

An object that represents a normalized point in an image, along with an identifier label and a confidence value.

struct VNRecognizedPointGroupKey

The data type for all recognized-point group keys.

