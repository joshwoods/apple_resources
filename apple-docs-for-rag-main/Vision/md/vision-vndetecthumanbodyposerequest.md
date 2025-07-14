

- Vision
-  VNDetectHumanBodyPoseRequest 

Class

# VNDetectHumanBodyPoseRequest

A request that detects a human body pose.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
class VNDetectHumanBodyPoseRequest
```

## Mentioned in 

Detecting Human Body Poses in Images

## Overview

The framework provides the detected body pose as a VNHumanBodyPoseObservation.

## Topics

### Determining Supported Joints

var supportedJointNames: [VNHumanBodyPoseObservation.JointName]

Retrieves the supported joint names.

class func supportedJointNames(forRevision: Int) throws -> [VNHumanBodyPoseObservation.JointName]

Retrieves the supported joint names for a revision.

Deprecated

var supportedJointsGroupNames: [VNHumanBodyPoseObservation.JointsGroupName]

Retrieves the supported joint group names.

class func supportedJointsGroupNames(forRevision: Int) throws -> [VNHumanBodyPoseObservation.JointsGroupName]

Retrieves the supported joint group names for a revision.

Deprecated

### Accessing the Results

var results: [VNHumanBodyPoseObservation]?

The observed body poses.

### Identifying Body Pose Revisions

let VNDetectHumanBodyPoseRequestRevision1: Int

A constant for specifying revision 1 of the body pose detection request.

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

### Body and hand pose detection

Detecting Human Body Poses in Images

Add the capability to detect human body poses to your app using the Vision framework.

Detecting Hand Poses with Vision

Create a virtual drawing app by using Vision’s capability to detect hand poses.

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

struct VNRecognizedPointKey

The data type for all recognized point keys.

struct VNRecognizedPointGroupKey

The data type for all recognized-point group keys.

