

- Vision
-  GenerateForegroundInstanceMaskRequest 

Structure

# GenerateForegroundInstanceMaskRequest

A request that generates an instance mask of noticeable objects to separate from the background.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
struct GenerateForegroundInstanceMaskRequest
```

## Overview

This request generates an InstanceMaskObservation object with instance-mask data.

## Topics

### Creating a request

init(GenerateForegroundInstanceMaskRequest.Revision?)

Creates a foreground instance-mask request.

### Getting the revision

let revision: GenerateForegroundInstanceMaskRequest.Revision

The algorithm or implementation the request uses.

static let supportedRevisions: [GenerateForegroundInstanceMaskRequest.Revision]

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

### Image feature print and background removal

struct GenerateImageFeaturePrintRequest

An image-based request to generate feature prints from an image.

