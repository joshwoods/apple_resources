

- Vision
-  VNRecognizedPoints3DObservation 

Class

# VNRecognizedPoints3DObservation

An observation that provides the 3D points for a request.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
class VNRecognizedPoints3DObservation
```

## Topics

### Inspecting the Observation

var availableKeys: [VNRecognizedPointKey]

The available point keys in the observation.

var availableGroupKeys: [VNRecognizedPointGroupKey]

The available point group keys in the observation.

func recognizedPoint(forKey: VNRecognizedPointKey) throws -> VNRecognizedPoint3D

Returns a point for a key you specify.

func recognizedPoints(forGroupKey: VNRecognizedPointGroupKey) throws -> [VNRecognizedPointKey : VNRecognizedPoint3D]

Returns a point for a group key you specify.

## Relationships

### Inherits From

- VNObservation

### Inherited By

- VNHumanBodyPose3DObservation

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

### 3D body pose detection

Identifying 3D human body poses in images

Detect three-dimensional human body poses using the Vision framework.

Detecting human body poses in 3D with Vision

Render skeletons of 3D body pose points in a scene overlaying the input image.

class VNDetectHumanBodyPose3DRequest

A request that detects points on human bodies in 3D space, relative to the camera.

class VNHumanBodyPose3DObservation

An observation that provides the 3D body points the request recognizes.

class VNHumanBodyRecognizedPoint3D

A recognized 3D point that includes a parent joint.

class VNPoint3D

An object that represents a 3D point in an image.

class VNRecognizedPoint3D

A 3D point that includes an identifier to the point.

struct JointName

The joint names for a 3D body pose.

struct JointsGroupName

The joint group names for a 3D body pose.

