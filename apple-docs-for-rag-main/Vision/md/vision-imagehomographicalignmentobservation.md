

- Vision
-  ImageHomographicAlignmentObservation 

Structure

# ImageHomographicAlignmentObservation

An object that represents a perspective warp transformation.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
struct ImageHomographicAlignmentObservation
```

## Overview

This type of observation results from a TrackHomographicImageRegistrationRequest, informing the warpTransform performed to align the input images.

## Topics

### Creating an observation

init(VNImageHomographicAlignmentObservation)

Creates a homographic alignment observation.

### Inspecting an observation

let warpTransform: matrix_float3x3

The warp transform matrix to morph the floating image into the reference image.

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

