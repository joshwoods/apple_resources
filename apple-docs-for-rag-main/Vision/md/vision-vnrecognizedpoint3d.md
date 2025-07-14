

- Vision
-  VNRecognizedPoint3D 

Class

# VNRecognizedPoint3D

A 3D point that includes an identifier to the point.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
class VNRecognizedPoint3D
```

## Topics

### Getting the Identifier

var identifier: VNRecognizedPointKey

The identifier that provides context about what kind of point the request recognizes.

## Relationships

### Inherits From

- VNPoint3D

### Inherited By

- VNHumanBodyRecognizedPoint3D

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

## See Also

### 3D body pose detection

Identifying 3D human body poses in images

Detect three-dimensional human body poses using the Vision framework.

Detecting human body poses in 3D with Vision

Render skeletons of 3D body pose points in a scene overlaying the input image.

class VNDetectHumanBodyPose3DRequest

A request that detects points on human bodies in 3D space, relative to the camera.

class VNHumanBodyPose3DObservation

An observation that provides the 3D body points the request recognizes.

class VNRecognizedPoints3DObservation

An observation that provides the 3D points for a request.

class VNHumanBodyRecognizedPoint3D

A recognized 3D point that includes a parent joint.

class VNPoint3D

An object that represents a 3D point in an image.

struct JointName

The joint names for a 3D body pose.

struct JointsGroupName

The joint group names for a 3D body pose.

