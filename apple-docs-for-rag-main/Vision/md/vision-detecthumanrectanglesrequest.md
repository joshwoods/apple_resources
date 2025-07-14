

- Vision
-  DetectHumanRectanglesRequest 

Structure

# DetectHumanRectanglesRequest

A request that finds rectangular regions that contain people in an image.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
struct DetectHumanRectanglesRequest
```

## Overview

The request returns the resulting rectangle data in a collection of HumanObservation objects.

## Topics

### Creating a request

init(DetectHumanRectanglesRequest.Revision?)

Creates a human detection request.

### Getting the revision

let revision: DetectHumanRectanglesRequest.Revision

The algorithm or implementation the request uses.

static let supportedRevisions: [DetectHumanRectanglesRequest.Revision]

The collection of revisions the request supports.

enum Revision

A type that describes the algorithm or implementation that the request performs.

### Inspecting a request

var upperBodyOnly: Bool

A Boolean value that indicates whether the request requires only detecting a human upper body to produce a result.

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

struct HumanObservation

An object that represents a person that the request detects.

## Relationships

### Conforms To

- CustomStringConvertible
- Equatable
- Hashable
- ImageProcessingRequest
- Sendable
- VisionRequest

## See Also

### Face and body detection

Analyzing a selfie and visualizing its content

Calculate face-capture quality and visualize facial features for a collection of images using the Vision framework.

struct DetectFaceRectanglesRequest

A request that finds faces within an image.

struct DetectFaceLandmarksRequest

An image-analysis request that finds facial features like eyes and mouth in an image.

struct DetectFaceCaptureQualityRequest

A request that produces a floating-point number that represents the capture quality of a face in a photo.

