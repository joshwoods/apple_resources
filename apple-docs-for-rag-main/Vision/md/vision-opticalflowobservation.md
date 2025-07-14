

- Vision
-  OpticalFlowObservation 

Structure

# OpticalFlowObservation

An object that represents an optical flow that an image-analysis request produces.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
struct OpticalFlowObservation
```

## Overview

The optical flow is a 2D image, with each pixel representing the directional change from a previous to current image.

## Topics

### Creating an observation

init?(VNPixelBufferObservation)

Creates an optical flow observation.

### Inspecting an observation

var pixelFormat: OSType

The four-character code that identifies the pixel format.

var size: CGSize

The size of the observation image.

### Getting the optical flow

func flow(at: NormalizedPoint) -> (Float, Float)

Returns the optical flow for the specified location in the observation image.

### Accessing the memory

func withUnsafePointer&lt;R>((UnsafeRawPointer) -> R) -> R

Invokes the given closure with a pointer to the given argument.

## Relationships

### Conforms To

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

