

- Vision
-  VNDetectHumanBodyPose3DRequest 

Class

# VNDetectHumanBodyPose3DRequest

A request that detects points on human bodies in 3D space, relative to the camera.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
class VNDetectHumanBodyPose3DRequest
```

## Mentioned in 

Identifying 3D human body poses in images

## Overview

This request generates a collection of VNHumanBodyPose3DObservation objects that describe the position of each body the request detects. If the system allows it, the request uses AVDepthData information to improve the accuracy.

## Topics

### Initializing a Request

init()

Creates a new request with no completion handler.

init(completionHandler: VNRequestCompletionHandler?)

Creates a new 3D body pose request with a completion handler.

### Determining Supported Joints

var supportedJointsGroupNames: [VNHumanBodyPose3DObservation.JointsGroupName]

Returns the joint names the request supports.

var supportedJointNames: [VNHumanBodyPose3DObservation.JointName]

Returns the joint group names the request supports.

### Accessing the Results

var results: [VNHumanBodyPose3DObservation]?

The 3D body pose the request observes.

## Relationships

### Inherits From

- VNStatefulRequest

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### 3D body pose detection

Identifying 3D human body poses in images

Detect three-dimensional human body poses using the Vision framework.

Detecting human body poses in 3D with Vision

Render skeletons of 3D body pose points in a scene overlaying the input image.

class VNHumanBodyPose3DObservation

An observation that provides the 3D body points the request recognizes.

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

