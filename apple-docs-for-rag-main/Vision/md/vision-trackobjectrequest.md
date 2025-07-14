

- Vision
-  TrackObjectRequest 

Class

# TrackObjectRequest

An image-analysis request that tracks the movement of a previously identified object across multiple images or video frames.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
final class TrackObjectRequest
```

## Overview

Use this type of request to track the bounding boxes around objects previously identified in an image. Vision attempts to locate the same object from the input observation throughout the sequence. The request returns the resulting rectangle data in an instance of RectangleObservation.

## Topics

### Creating a request

init(detectedObject: any BoundingBoxProviding &amp; VisionObservation, TrackObjectRequest.Revision?, frameAnalysisSpacing: CMTime?)

Creates an object tracking request.

protocol BoundingBoxProviding

A protocol for objects that have a bounding box.

### Getting the revision

let revision: TrackObjectRequest.Revision

The algorithm or implementation the request uses.

static let supportedRevisions: [TrackObjectRequest.Revision]

The collection of revisions the request supports.

enum Revision

A type that describes the algorithm or implementation that the request performs.

### Inspecting a request

let inputObservation: any BoundingBoxProviding &amp; VisionObservation

The object to track.

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

struct DetectedObjectObservation

An observation that provides the position and extent of an image feature that an image-analysis request detects.

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

### Object tracking

class TrackRectangleRequest

An image-analysis request that tracks movement of a previously identified rectangular object across multiple images or video frames.

