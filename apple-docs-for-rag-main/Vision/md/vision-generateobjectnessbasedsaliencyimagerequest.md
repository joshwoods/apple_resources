

- Vision
-  GenerateObjectnessBasedSaliencyImageRequest 

Structure

# GenerateObjectnessBasedSaliencyImageRequest

A request that generates a heat map that identifies the parts of an image most likely to represent objects.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
struct GenerateObjectnessBasedSaliencyImageRequest
```

## Overview

The request returns the resulting heat map and object data in an instance of SaliencyImageObservation.

## Topics

### Creating a request

init(GenerateObjectnessBasedSaliencyImageRequest.Revision?)

Creates an objectness saliency image request.

### Getting the revision

let revision: GenerateObjectnessBasedSaliencyImageRequest.Revision

The algorithm or implementation the request uses.

static let supportedRevisions: [GenerateObjectnessBasedSaliencyImageRequest.Revision]

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

struct SaliencyImageObservation

An observation that contains a grayscale heat map of important areas across an image.

## Relationships

### Conforms To

- CustomStringConvertible
- Equatable
- Hashable
- ImageProcessingRequest
- Sendable
- VisionRequest

## See Also

### Saliency analysis

struct GenerateAttentionBasedSaliencyImageRequest

An object that produces a heat map that identifies the parts of an image most likely to draw attention.

