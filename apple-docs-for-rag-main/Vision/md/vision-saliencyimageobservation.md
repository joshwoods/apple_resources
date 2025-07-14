

- Vision
-  SaliencyImageObservation 

Structure

# SaliencyImageObservation

An observation that contains a grayscale heat map of important areas across an image.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
struct SaliencyImageObservation
```

## Topics

### Creating an observation

init?(VNSaliencyImageObservation)

Creates a saliency image observation.

### Inspecting an observation

enum RequestDescriptor

A type that describes the request and revision combination.

let heatMap: PixelBufferObservation

A grayscale heat map of important areas across the image.

struct PixelBufferObservation

An object that represents an image that an image-analysis request produces.

let salientObjects: [RectangleObservation]

A collection of objects describing the distinct areas of the saliency heat map.

struct RectangleObservation

An object that represents the four vertices of a detected rectangle.

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

