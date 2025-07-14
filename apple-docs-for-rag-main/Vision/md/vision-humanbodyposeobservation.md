

- Vision
-  HumanBodyPoseObservation 

Structure

# HumanBodyPoseObservation

An observation that provides the body points the analysis recognizes.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
struct HumanBodyPoseObservation
```

## Topics

### Creating an observation

init(VNHumanBodyPoseObservation)

Creates a human body pose observation.

### Inspecting an observation

enum RequestDescriptor

A type that describes the request and revision combination.

let leftHand: HumanHandPoseObservation?

The observed left hand.

let rightHand: HumanHandPoseObservation?

The observed right hand.

struct HumanHandPoseObservation

An observation that provides the hand points the analysis recognizes.

var keypoints: MLMultiArray

A multi-array compatible with Core ML that contains normalized point coordinates and confidence scores.

### Getting the joints

enum JointsGroupName

The joint group names available in the observation.

enum JointName

The supported joint names for the body pose.

## Relationships

### Conforms To

- Copyable
- CustomStringConvertible
- Decodable
- Encodable
- Equatable
- Hashable
- PoseProviding
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

