

- Vision
-  DetectHumanBodyPose3DRequest 

Class

# DetectHumanBodyPose3DRequest

A request that detects points on human bodies in 3D space, relative to the camera.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
final class DetectHumanBodyPose3DRequest
```

## Overview

This request generates a collection of HumanBodyPose3DObservation objects that describe the position of each body the request detects. If the system allows it, the request uses AVDepthData information to improve the accuracy.

## Topics

### Creating a request

init(DetectHumanBodyPose3DRequest.Revision?, frameAnalysisSpacing: CMTime?)

Creates a 3D human body pose request.

### Getting the revision

let revision: DetectHumanBodyPose3DRequest.Revision

The algorithm or implementation the request uses.

static let supportedRevisions: [DetectHumanBodyPose3DRequest.Revision]

The collection of revisions the request supports.

enum Revision

A type that describes the algorithm or implementation that the request performs.

### Inspecting a request

var supportedJointNames: [HumanBodyPose3DObservation.JointName]

The joint names the request supports.

var supportedJointsGroupNames: [HumanBodyPose3DObservation.JointsGroupName]

The joint group names the request supports.

### Performing a request

func perform(on: URL, orientation: CGImagePropertyOrientation?) async throws -> Self.Result

Performs the request on an image URL and produces observations.

**Required** Default implementations provided.

func perform(on: Data, orientation: CGImagePropertyOrientation?) async throws -> Self.Result

Performs the request on image data and produces observations.

**Required** Default implementations provided.

func perform(on: CGImage, orientation: CGImagePropertyOrientation?) async throws -> Self.Result

Performs the request on a Core Graphics image and produces observations.

**Required** Default implementations provided.

func perform(on: CVPixelBuffer, orientation: CGImagePropertyOrientation?) async throws -> Self.Result

Performs the request on a pixel buffer and produces observations.

**Required** Default implementations provided.

func perform(on: CMSampleBuffer, orientation: CGImagePropertyOrientation?) async throws -> Self.Result

Performs the request on a Core Media buffer and produces observations.

**Required** Default implementations provided.

func perform(on: CIImage, orientation: CGImagePropertyOrientation?) async throws -> Self.Result

Performs the request on a Core Image image and produces observations.

**Required** Default implementations provided.

struct HumanBodyPose3DObservation

An observation that provides the 3D body points the request recognizes.

## Relationships

### Conforms To

- CustomStringConvertible
- Equatable
- Hashable
- ImageProcessingRequest
- Sendable
- StatefulRequest
- VisionRequest

## See Also

### 3D body pose detection

struct Joint3D

An object that represents a body pose joint in 3D space.

