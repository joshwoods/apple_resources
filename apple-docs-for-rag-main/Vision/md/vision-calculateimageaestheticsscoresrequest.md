

- Vision
-  CalculateImageAestheticsScoresRequest 

Structure

# CalculateImageAestheticsScoresRequest

A request that analyzes an image for aesthetically pleasing attributes.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
struct CalculateImageAestheticsScoresRequest
```

## Overview

The request returns the resulting aesthetics score in an instance of ImageAestheticsScoresObservation.

## Topics

### Creating a request

init(CalculateImageAestheticsScoresRequest.Revision?)

Creates an image aesthetics request.

### Getting the revision

let revision: CalculateImageAestheticsScoresRequest.Revision

The algorithm or implementation the request uses.

static let supportedRevisions: [CalculateImageAestheticsScoresRequest.Revision]

The collection of revisions the request supports.

enum Revision

A type that describes the algorithm or implementation that the request performs.

### Inspecting a request

var cropAndScaleAction: ImageCropAndScaleAction

An optional setting that tells the algorithm how to scale an input image before generating the result.

enum ImageCropAndScaleAction

A scale to apply to an input image before performing a request.

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

struct ImageAestheticsScoresObservation

An observation that provides an overall score of aesthetic attributes for an image.

## Relationships

### Conforms To

- CustomStringConvertible
- Equatable
- Hashable
- ImageProcessingRequest
- Sendable
- VisionRequest

## See Also

### Image aesthetics analysis

Generating high-quality thumbnails from videos

Identify the most visually pleasing frames in a video by using the image-aesthetics scores request.

