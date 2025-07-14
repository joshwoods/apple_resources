

- Vision
-  InstanceMaskObservation 

Structure

# InstanceMaskObservation

An observation that contains an instance mask that labels instances in the mask.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
struct InstanceMaskObservation
```

## Topics

### Creating an observation

init?(VNInstanceMaskObservation)

Creates an instance mask observation.

### Inspecting an observation

enum RequestDescriptor

A type that describes the request and revision combination.

### Generating a mask

func generateMask(for: IndexSet) throws -> CVPixelBuffer

Creates a low-resolution mask from the instances you specify.

func generateMaskedImage(for: IndexSet, imageFrom: ImageRequestHandler, croppedToInstancesExtent: Bool) throws -> CVPixelBuffer

Creates a high-resolution image with everything except for the instances you specify masked out.

func generateScaledMask(for: IndexSet, scaledToImageFrom: ImageRequestHandler) throws -> CVPixelBuffer

Creates a high-resolution mask representing a combination of the instances you specify.

### Getting instances

func instanceAtPoint(NormalizedPoint) -> IndexSet

Returns an instance at the point you specify.

let allInstances: IndexSet

The collection that contains all instances, excluding the background.

let allInstancesMask: PixelBufferObservation

The resulting mask that represents all instances.

struct PixelBufferObservation

An object that represents an image that an image-analysis request produces.

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

