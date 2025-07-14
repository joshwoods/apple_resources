

- Vision
-  PixelBufferObservation 

Structure

# PixelBufferObservation

An object that represents an image that an image-analysis request produces.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
struct PixelBufferObservation
```

## Topics

### Creating an observation

init?(VNPixelBufferObservation)

Creates a pixel buffer observation.

### Inspecting an observation

enum RequestDescriptor

A type that describes the request and revision combination.

var cgImage: CGImage

A Core Graphics image created from the pixel buffer observation.

var pixelFormat: OSType

The four-character code that identifies the pixel format.

var size: CGSize

The size of the image.

### Getting pixel data

func pixel(at: NormalizedPoint) -> Float

Returns the pixel data for the specified location in the image.

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

### Machine learning image analysis

struct CoreMLRequest

An image-analysis request that uses a Core ML model to process images.

struct CoreMLFeatureValueObservation

An object that represents a collection of key-value information that a Core ML image-analysis request produces.

struct ClassificationObservation

An object that represents classification information that an image-analysis request produces.

