

- Vision
-  ImageTranslationAlignmentObservation 

Structure

# ImageTranslationAlignmentObservation

Affine transform information that an image-alignment request produces.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
struct ImageTranslationAlignmentObservation
```

## Overview

This type of observation results from a TrackTranslationalImageRegistrationRequest, informing the alignmentTransform performed to align the input images.

## Topics

### Creating an observation

init(VNImageTranslationAlignmentObservation)

Creates a translation alignment observation.

### Inspecting an observation

let alignmentTransform: CGAffineTransform

The alignment transform to align the floating image with the reference image.

### Applying a transform

func applyTransform(to: CIImage) -> CIImage

Applies the transform to an image.

## Relationships

### Conforms To

- Copyable
- CustomStringConvertible
- Decodable
- Encodable
- Equatable
- Hashable
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

