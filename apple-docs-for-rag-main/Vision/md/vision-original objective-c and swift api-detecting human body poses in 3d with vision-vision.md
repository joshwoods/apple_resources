

- Vision
- Original Objective-C and Swift API
-  Detecting human body poses in 3D with Vision 

Sample Code

# Detecting human body poses in 3D with Vision

Render skeletons of 3D body pose points in a scene overlaying the input image.

Download

iOS 17.0+iPadOS 17.0+Xcode 15.0+

## Overview

Note

This sample code project is associated with WWDC23 session 111241: Explore 3D body pose and person segmentation in Vision.

### Configure the sample code project

Before you run the sample code project in Xcode, ensure you’re using an iOS device with an A12 chip or later. The input image should have all limbs of the subject visible.

Note

Due to a behavior change with `cameraOriginMatrix` API, if this sample project is run on a device on a build earlier than beta 3, camera position will be rotated 180 degrees.

## See Also

### 3D body pose detection

Identifying 3D human body poses in images

Detect three-dimensional human body poses using the Vision framework.

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

class VNRecognizedPoint3D

A 3D point that includes an identifier to the point.

struct JointName

The joint names for a 3D body pose.

struct JointsGroupName

The joint group names for a 3D body pose.

