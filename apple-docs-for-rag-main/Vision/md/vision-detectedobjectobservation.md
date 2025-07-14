

- Vision
-  DetectedObjectObservation 

Structure

# DetectedObjectObservation

An observation that provides the position and extent of an image feature that an image-analysis request detects.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
struct DetectedObjectObservation
```

## Overview

This class is the observation type that TrackObjectRequest generates. It represents an object that the Vision request detects and tracks.

## Topics

### Creating an observation

init(VNDetectedObjectObservation)

Creates a detected object observation.

init(boundingBox: NormalizedRect)

Creates a detected object observation with the bounding box you specify.

### Inspecting an observation

enum RequestDescriptor

A type that describes the request and revision combination.

## Relationships

### Conforms To

- BoundingBoxProviding
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

