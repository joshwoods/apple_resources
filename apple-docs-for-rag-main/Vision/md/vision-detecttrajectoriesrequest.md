

- Vision
-  DetectTrajectoriesRequest 

Class

# DetectTrajectoriesRequest

A request that detects the trajectories of shapes moving along a parabolic path.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
final class DetectTrajectoriesRequest
```

## Overview

After the request detects a trajectory, it produces a collection of TrajectoryObservation objects that contain the shape’s detected points and an equation describing the parabola.

## Topics

### Creating a request

init(trajectoryLength: Int, DetectTrajectoriesRequest.Revision?, frameAnalysisSpacing: CMTime?)

Creates a trajectory-detection request.

### Getting the revision

let revision: DetectTrajectoriesRequest.Revision

The algorithm or implementation the request uses.

static let supportedRevisions: [DetectTrajectoriesRequest.Revision]

The collection of revisions the request supports.

enum Revision

A type that describes the algorithm or implementation that the request performs.

### Inspecting a request

var objectMaximumNormalizedRadius: Float

The maximum radius of the bounding circle of the object to track.

var objectMinimumNormalizedRadius: Float

The minimum radius of the bounding circle of the object to track.

var targetFrameTime: CMTime

The requested target frame time for processing trajectory detection.

let trajectoryLength: Int

The number of points to detect before calculating a trajectory.

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

struct TrajectoryObservation

An observation that describes a detected trajectory.

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

### Trajectory, contour, and horizon detection

struct DetectContoursRequest

A request that detects the contours of the edges of an image.

struct DetectHorizonRequest

An image-analysis request that determines the horizon angle in an image.

