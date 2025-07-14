

- Vision
-  VNDetectHumanHandPoseRequest 

Class

# VNDetectHumanHandPoseRequest

A request that detects a human hand pose.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
class VNDetectHumanHandPoseRequest
```

## Overview

The framework provides the detected hand pose as a `VNIdentifiedPointsObservation`.

## Topics

### Configuring the Request

var maximumHandCount: Int

The maximum number of hands to detect in an image.

### Determining Supported Joints

var supportedJointNames: [VNHumanHandPoseObservation.JointName]

Retrieves the supported joint names.

class func supportedJointNames(forRevision: Int) throws -> [VNHumanHandPoseObservation.JointName]

Retrieves the supported joint names for a revision.

Deprecated

var supportedJointsGroupNames: [VNHumanHandPoseObservation.JointsGroupName]

Retrieves the supported joint group names.

class func supportedJointsGroupNames(forRevision: Int) throws -> [VNHumanHandPoseObservation.JointsGroupName]

Retrieves the supported joint group names for a revision.

Deprecated

### Accessing the Results

var results: [VNHumanHandPoseObservation]?

The observed hand poses.

### Identifying Hand Pose Revisions

let VNDetectHumanHandPoseRequestRevision1: Int

A constant for specifying revision 1 of the hand pose detection request.

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

class VNDetectHumanBodyPoseRequest

A request that detects a human body pose.

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

