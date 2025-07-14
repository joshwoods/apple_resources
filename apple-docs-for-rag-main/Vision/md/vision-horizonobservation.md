

- Vision
-  HorizonObservation 

Structure

# HorizonObservation

The horizon angle information that an image-analysis request detects.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
struct HorizonObservation
```

## Overview

Instances of this class result from invoking a DetectHorizonRequest, and report the angle and transform of the horizon in an image.

## Topics

### Creating an observation

init(VNHorizonObservation)

Creates a horizon observation.

### Inspecting an observation

let angle: Measurement&lt;UnitAngle>

The angle of the observed horizon.

### Getting the transform

let transform: CGAffineTransform

The transform to apply to the detected horizon.

func transform(for: CGSize) -> CGAffineTransform

Creates an affine transform for the specified image width and height.

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

