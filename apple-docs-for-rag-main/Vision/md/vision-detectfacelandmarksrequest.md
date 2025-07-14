

- Vision
-  DetectFaceLandmarksRequest 

Structure

# DetectFaceLandmarksRequest

An image-analysis request that finds facial features like eyes and mouth in an image.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
struct DetectFaceLandmarksRequest
```

## Overview

By default, a request for face landmarks first locates all faces in the input image, then analyzes each to detect facial features.

If you already located all the faces in an image, or want to detect landmarks in only a subset of the faces in the image, set the inputFaceObservations property to an array of FaceObservation objects representing the faces you want to analyze. You can either use face observations output by a DetectFaceRectanglesRequest or manually create FaceObservation instances with the bounding boxes of the faces you want to analyze.

## Topics

### Creating a request

init(DetectFaceLandmarksRequest.Revision?)

Creates a face landmark detection request.

### Getting the revision

let revision: DetectFaceLandmarksRequest.Revision

The algorithm or implementation the request uses.

static let supportedRevisions: [DetectFaceLandmarksRequest.Revision]

The collection of revisions the request supports.

enum Revision

A type that describes the algorithm or implementation that the request performs.

### Inspecting a request

var inputFaceObservations: [FaceObservation]?

An array of face-observation objects to process as part of the request.

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

struct FaceObservation

An image-analysis request that identifies facial features in an image.

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

struct DetectFaceCaptureQualityRequest

A request that produces a floating-point number that represents the capture quality of a face in a photo.

struct DetectHumanRectanglesRequest

A request that finds rectangular regions that contain people in an image.

