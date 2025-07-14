

- Vision
-  DetectContoursRequest 

Structure

# DetectContoursRequest

A request that detects the contours of the edges of an image.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
struct DetectContoursRequest
```

## Overview

This request generates a ContoursObservation object that describes the contours in an image.

## Topics

### Creating a request

init(DetectContoursRequest.Revision?)

Creates a contour-detection request.

### Getting the revision

let revision: DetectContoursRequest.Revision

The algorithm or implementation the request uses.

static let supportedRevisions: [DetectContoursRequest.Revision]

The collection of revisions the request supports.

enum Revision

A type that describes the algorithm or implementation that the request performs.

### Inspecting a request

var contrastAdjustment: Float

The amount by which to adjust the image contrast.

var contrastPivot: Float?

The pixel value to use as a pivot for the contrast.

var detectsDarkOnLight: Bool

A Boolean value that indicates whether the request detects a dark object on a light background to aid in detection.

var maximumImageDimension: Int

The maximum image dimension to use for contour detection.

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

struct ContoursObservation

An object that represents the detected contours in an image.

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

struct DetectHorizonRequest

An image-analysis request that determines the horizon angle in an image.

