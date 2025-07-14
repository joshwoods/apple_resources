

- Vision
-  TrackRectangleRequest 

Class

# TrackRectangleRequest

An image-analysis request that tracks movement of a previously identified rectangular object across multiple images or video frames.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
final class TrackRectangleRequest
```

## Overview

Use this type of request to track the bounding boxes of rectangles throughout a sequence of images. Vision returns locations for rectangles found in all orientations and sizes. The request returns the resulting rectangle data in an instance of RectangleObservation.

## Topics

### Creating a request

init(detectedRectangle: any QuadrilateralProviding &amp; VisionObservation, TrackRectangleRequest.Revision?, frameAnalysisSpacing: CMTime?)

Creates a rectangle tracking request.

### Getting the revision

let revision: TrackRectangleRequest.Revision

The algorithm or implementation the request uses.

static let supportedRevisions: [TrackRectangleRequest.Revision]

The collection of revisions the request supports.

enum Revision

A type that describes the algorithm or implementation that the request performs.

### Inspecting a request

let inputObservation: any QuadrilateralProviding &amp; VisionObservation

The object to track.

protocol QuadrilateralProviding

A protocol for objects that have a bounding quadrilateral.

var trackingLevel: TrackRectangleRequest.TrackingLevel

The tracking quality preference.

enum TrackingLevel

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

struct RectangleObservation

An object that represents the four vertices of a detected rectangle.

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

class TrackObjectRequest

An image-analysis request that tracks the movement of a previously identified object across multiple images or video frames.

