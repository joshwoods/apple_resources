

- Vision
-  FaceObservation 

Structure

# FaceObservation

An image-analysis request that identifies facial features in an image.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
struct FaceObservation
```

## Topics

### Creating an observation

init(VNFaceObservation)

Creates a face observation.

init(boundingBox: NormalizedRect, revision: DetectFaceRectanglesRequest.Revision?)

Creates a face observation from its bounding box.

### Inspecting an observation

enum RequestDescriptor

A type that describes the request and revision combination.

struct Landmarks2D

A collection of facial features that a request detects.

let landmarks: FaceObservation.Landmarks2D?

The facial features of the detected face.

let pitch: Measurement&lt;UnitAngle>

The pitch angle of a face.

let roll: Measurement&lt;UnitAngle>

The roll angle of a face.

let yaw: Measurement&lt;UnitAngle>

The yaw angle of a face.

### Structures

struct CaptureQuality

An indicator of the quality of a face capture.

### Instance Properties

let captureQuality: FaceObservation.CaptureQuality?

The quality of the face capture.

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

