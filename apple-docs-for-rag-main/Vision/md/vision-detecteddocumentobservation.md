

- Vision
-  DetectedDocumentObservation 

Structure

# DetectedDocumentObservation

The heat map that’s a pixel buffer in a one-component floating-point pixel format.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
struct DetectedDocumentObservation
```

## Overview

The observation includes the four corner points of a document’s quadrilateral and saliency masks.

## Topics

### Creating an observation

init?(VNRectangleObservation)

Creates a detected document observation.

### Inspecting an observation

enum RequestDescriptor

A type that describes the request and revision combination.

var globalSegmentationMask: PixelBufferObservation

A pixel buffer representing a segmentation mask for the detected document.

struct PixelBufferObservation

An object that represents an image that an image-analysis request produces.

## Relationships

### Conforms To

- BoundingBoxProviding
- Copyable
- CustomStringConvertible
- Decodable
- Encodable
- Equatable
- Hashable
- QuadrilateralProviding
- Sendable
- VisionObservation

## See Also

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

