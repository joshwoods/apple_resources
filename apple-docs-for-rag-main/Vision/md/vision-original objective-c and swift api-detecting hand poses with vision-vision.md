

- Vision
- Original Objective-C and Swift API
-  Detecting Hand Poses with Vision 

Sample Code

# Detecting Hand Poses with Vision

Create a virtual drawing app by using Vision’s capability to detect hand poses.

Download

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+Xcode 12.0+

## Overview

Note

This sample code project is associated with WWDC20 session 10653: Detect Body and Hand Pose with Vision.

## See Also

### Body and hand pose detection

Detecting Human Body Poses in Images

Add the capability to detect human body poses to your app using the Vision framework.

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

struct VNRecognizedPointKey

The data type for all recognized point keys.

struct VNRecognizedPointGroupKey

The data type for all recognized-point group keys.

