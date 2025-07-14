

- Vision
-  DetectHorizonRequest 

Structure

# DetectHorizonRequest

An image-analysis request that determines the horizon angle in an image.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
struct DetectHorizonRequest
```

## Overview

This request generates a HorizonObservation object that describes the horizon the request detects.

## Topics

### Creating a request

init(DetectHorizonRequest.Revision?)

Creates a horizon-detection request.

### Getting the revision

let revision: DetectHorizonRequest.Revision

The algorithm or implementation the request uses.

static let supportedRevisions: [DetectHorizonRequest.Revision]

The collection of revisions the request supports.

enum Revision

A type that describes the algorithm or implementation that the request performs.

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

struct HorizonObservation

The horizon angle information that an image-analysis request detects.

## Relationships

### Conforms To

- CustomStringConvertible
- Equatable
- Hashable
- ImageProcessingRequest
- Sendable
- VisionRequest

## See Also

### Trajectory, contour, and horizon detection

class DetectTrajectoriesRequest

A request that detects the trajectories of shapes moving along a parabolic path.

struct DetectContoursRequest

A request that detects the contours of the edges of an image.

