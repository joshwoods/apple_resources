

- Vision
-  GeneratePersonInstanceMaskRequest 

Structure

# GeneratePersonInstanceMaskRequest

A request that produces a mask of individual people it finds in the input image.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
struct GeneratePersonInstanceMaskRequest
```

## Overview

The request returns the resulting image mask in an instance of InstanceMaskObservation.

## Topics

### Creating a request

init(GeneratePersonInstanceMaskRequest.Revision?)

Creates a person instance mask request.

### Getting the revision

let revision: GeneratePersonInstanceMaskRequest.Revision

The algorithm or implementation the request uses.

static let supportedRevisions: [GeneratePersonInstanceMaskRequest.Revision]

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

struct InstanceMaskObservation

An observation that contains an instance mask that labels instances in the mask.

## Relationships

### Conforms To

- CustomStringConvertible
- Equatable
- Hashable
- ImageProcessingRequest
- Sendable
- VisionRequest

## See Also

### Image sequence analysis

class GeneratePersonSegmentationRequest

A request that produces a matte image for a person it finds in the input image.

struct DetectDocumentSegmentationRequest

A request that detects rectangular regions that contain text in the input image.

protocol StatefulRequest

The protocol for a type that builds evidence of a condition over time.

