

- Vision
-  DetectTextRectanglesRequest 

Structure

# DetectTextRectanglesRequest

An image-analysis request that finds regions of visible text in an image.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
struct DetectTextRectanglesRequest
```

## Overview

This request generates a collection of TextObservation objects that describe each text region the request detects.

## Topics

### Creating a request

init(DetectTextRectanglesRequest.Revision?)

Creates a text rectangles detection request.

### Getting the revision

let revision: DetectTextRectanglesRequest.Revision

The algorithm or implementation the request uses.

static let supportedRevisions: [DetectTextRectanglesRequest.Revision]

The collection of revisions the request supports.

enum Revision

A type that describes the algorithm or implementation that the request performs.

### Inspecting a request

var reportCharacterBoxes: Bool

A Boolean value that indicates whether the request detects character-bounding boxes.

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

struct TextObservation

Information about regions of text that an image-analysis request detects.

## Relationships

### Conforms To

- CustomStringConvertible
- Equatable
- Hashable
- ImageProcessingRequest
- Sendable
- VisionRequest

## See Also

### Text detection

Locating and displaying recognized text

Perform text recognition on a photo using the Vision framework’s text-recognition request.

struct RecognizeTextRequest

An image-analysis request that recognizes text in an image.

