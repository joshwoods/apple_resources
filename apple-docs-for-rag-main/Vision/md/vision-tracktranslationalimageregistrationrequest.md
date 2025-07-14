

- Vision
-  TrackTranslationalImageRegistrationRequest 

Class

# TrackTranslationalImageRegistrationRequest

An image-analysis request that you track over time to determine the affine transform necessary to align the content of two images.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
final class TrackTranslationalImageRegistrationRequest
```

## Overview

This request generates an ImageTranslationAlignmentObservation object that describes the transform data the request detects.

## Topics

### Creating a request

init(TrackTranslationalImageRegistrationRequest.Revision?, frameAnalysisSpacing: CMTime?)

Creates an image-alignment tracking request to determine the affine transform.

### Getting the revision

let revision: TrackTranslationalImageRegistrationRequest.Revision

The algorithm or implementation the request uses.

static let supportedRevisions: [TrackTranslationalImageRegistrationRequest.Revision]

The collection of revisions the request supports.

enum Revision

A type that describes the algorithm or implementation that the request performs.

### Inspecting a request

enum ComputeStage

Types that represent the compute stage.

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

struct ImageTranslationAlignmentObservation

Affine transform information that an image-alignment request produces.

## Relationships

### Conforms To

- CustomStringConvertible
- Equatable
- Hashable
- ImageProcessingRequest
- Sendable
- StatefulRequest
- TargetedRequest
- VisionRequest

## See Also

### Image alignment

class TrackHomographicImageRegistrationRequest

An image-analysis request that you track over time to determine the perspective warp matrix necessary to align the content of two images.

protocol TargetedRequest

A type for analyzing two images together.

