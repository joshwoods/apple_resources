

- Vision
-  GeneratePersonSegmentationRequest 

Class

# GeneratePersonSegmentationRequest

A request that produces a matte image for a person it finds in the input image.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
final class GeneratePersonSegmentationRequest
```

## Overview

Perform this request to detect and generate an image mask for a person in an image. The request returns the resulting image mask in an instance of PixelBufferObservation.

## Topics

### Creating a request

init(GeneratePersonSegmentationRequest.Revision?, frameAnalysisSpacing: CMTime?)

Creates a person-segmentation request.

### Getting the revision

let revision: GeneratePersonSegmentationRequest.Revision

The algorithm or implementation the request uses.

static let supportedRevisions: [GeneratePersonSegmentationRequest.Revision]

The collection of revisions the request supports.

enum Revision

A type that describes the algorithm or implementation that the request performs.

### Inspecting a request

var qualityLevel: GeneratePersonSegmentationRequest.QualityLevel

A value that indicates how the request balances accuracy and performance.

enum QualityLevel

Constants that define the levels of quality for a person-segmentation request.

var outputPixelFormatType: OSType

The desired pixel format of the observation.

var supportedOutputPixelFormats: [OSType]

The collection of supported pixel format types.

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

struct PixelBufferObservation

An object that represents an image that an image-analysis request produces.

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

### Image sequence analysis

struct GeneratePersonInstanceMaskRequest

A request that produces a mask of individual people it finds in the input image.

struct DetectDocumentSegmentationRequest

A request that detects rectangular regions that contain text in the input image.

protocol StatefulRequest

The protocol for a type that builds evidence of a condition over time.

