

- Vision
-  VNHumanBodyPose3DObservation 

Class

# VNHumanBodyPose3DObservation

An observation that provides the 3D body points the request recognizes.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
class VNHumanBodyPose3DObservation
```

## Mentioned in 

Identifying 3D human body poses in images

## Topics

### Accessing Points

var availableJointNames: [VNHumanBodyPose3DObservation.JointName]

The names of the available joints in the observation.

struct JointName

The joint names for a 3D body pose.

var availableJointsGroupNames: [VNHumanBodyPose3DObservation.JointsGroupName]

The available joint group names in the observation.

struct JointsGroupName

The joint group names for a 3D body pose.

func recognizedPoint(VNHumanBodyPose3DObservation.JointName) throws -> VNHumanBodyRecognizedPoint3D

Returns the point for a joint name that the observation recognizes.

func recognizedPoints(VNHumanBodyPose3DObservation.JointsGroupName) throws -> [VNHumanBodyPose3DObservation.JointName : VNHumanBodyRecognizedPoint3D]

Returns a collection of points for the group name you specify.

### Getting the Joint Position

func pointInImage(VNHumanBodyPose3DObservation.JointName) throws -> VNPoint

Returns a 2D point for the joint name you specify, relative to the input image.

### Getting the Parent Joint Name

func parentJointName(VNHumanBodyPose3DObservation.JointName) -> VNHumanBodyPose3DObservation.JointName?

Returns the parent joint of the joint name you specify.

### Getting the Body Height

var heightEstimation: VNHumanBodyPose3DObservation.HeightEstimation

The technique the framework uses to estimate body height.

enum HeightEstimation

Constants that identify body height estimation techniques.

var bodyHeight: Float

The estimated human body height, in meters.

### Getting the Camera Position

var cameraOriginMatrix: simd_float4x4

A transform from the skeleton hip to the camera.

func cameraRelativePosition(VNHumanBodyPose3DObservation.JointName) throws -> simd_float4x4

Returns a position relative to the camera for the body joint you specify.

## Relationships

### Inherits From

- VNRecognizedPoints3DObservation

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

class VNRecognizedPoints3DObservation

An observation that provides the 3D points for a request.

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

