

- Vision
-  DetectAnimalBodyPoseRequest 

Structure

# DetectAnimalBodyPoseRequest

A request that detects an animal body pose.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
struct DetectAnimalBodyPoseRequest
```

## Overview

This request generates a collection of AnimalBodyPoseObservation objects that describe the position of each animal the request detects.

## Topics

### Creating a request

init(DetectAnimalBodyPoseRequest.Revision?)

Creates an animal body pose-detection request.

### Getting the revision

let revision: DetectAnimalBodyPoseRequest.Revision

The algorithm or implementation the request uses.

static let supportedRevisions: [DetectAnimalBodyPoseRequest.Revision]

The collection of revisions the request supports.

enum Revision

A type that describes the algorithm or implementation that the request performs.

### Inspecting a request

var supportedJointNames: [AnimalBodyPoseObservation.JointName]

The joint names the request supports.

var supportedJointsGroupNames: [AnimalBodyPoseObservation.JointsGroupName]

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

struct AnimalBodyPoseObservation

An observation that provides the animal body points the analysis recognizes.

## Relationships

### Conforms To

- CustomStringConvertible
- Equatable
- Hashable
- ImageProcessingRequest
- Sendable
- VisionRequest

## See Also

### Animal detection

struct RecognizeAnimalsRequest

A request that recognizes animals in an image.

