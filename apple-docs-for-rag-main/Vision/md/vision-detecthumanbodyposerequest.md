

- Vision
-  DetectHumanBodyPoseRequest 

Structure

# DetectHumanBodyPoseRequest

A request that detects a human body pose.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
struct DetectHumanBodyPoseRequest
```

## Overview

This type of request produces a collection of HumanBodyPoseObservation objects that describe the body pose.

## Topics

### Creating a request

init(DetectHumanBodyPoseRequest.Revision?)

Creates a human body pose request.

### Getting the revision

let revision: DetectHumanBodyPoseRequest.Revision

The algorithm or implementation the request uses.

static let supportedRevisions: [DetectHumanBodyPoseRequest.Revision]

The collection of revisions the request supports.

enum Revision

A type that describes the algorithm or implementation that the request performs.

### Inspecting a request

var detectsHands: Bool

A Boolean value that detects hands of the body in the results, if they’re visible.

var supportedJointNames: [HumanBodyPoseObservation.JointName]

The joint names the request supports.

var supportedJointsGroupNames: [HumanBodyPoseObservation.JointsGroupName]

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

struct HumanBodyPoseObservation

An observation that provides the body points the analysis recognizes.

## Relationships

### Conforms To

- CustomStringConvertible
- Equatable
- Hashable
- ImageProcessingRequest
- Sendable
- VisionRequest

## See Also

### Body and hand pose detection

struct DetectHumanHandPoseRequest

A request that detects a human hand pose.

protocol PoseProviding

An observation that provides a collection of joints that make up a pose.

enum Chirality

The hand sidedness of a pose.

struct Joint

A pose joint represented as a normalized point in an image, along with a label and a confidence value.

