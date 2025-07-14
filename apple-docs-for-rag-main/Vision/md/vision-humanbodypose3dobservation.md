

- Vision
-  HumanBodyPose3DObservation 

Structure

# HumanBodyPose3DObservation

An observation that provides the 3D body points the request recognizes.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
struct HumanBodyPose3DObservation
```

## Topics

### Creating an observation

init(VNHumanBodyPose3DObservation)

Creates a 3D human body pose observation.

### Inspecting an observation

enum RequestDescriptor

A type that describes the request and revision combination.

let bodyHeight: Measurement&lt;UnitLength>

The estimated human body height, in meters.

let cameraOriginMatrix: simd_float4x4

A transform from the skeleton hip to the camera.

enum EstimationTechnique

Constants that identify body height estimation techniques.

let heightEstimationTechnique: HumanBodyPose3DObservation.EstimationTechnique

The technique the framework uses to estimate body height.

### Getting the joints

func allJoints(in: HumanBodyPose3DObservation.JointsGroupName?) -> [HumanBodyPose3DObservation.JointName : Joint3D]

Retrieves a dictionary of all joints in a joint group.

var availableJointsGroupNames: [HumanBodyPose3DObservation.JointsGroupName]

The names of the available joint groupings in the observation.

enum JointsGroupName

The supported joint group names for the body pose.

func joint(for: HumanBodyPose3DObservation.JointName) -> Joint3D?

Retrieves a joint for a given joint name.

var availableJointNames: [HumanBodyPose3DObservation.JointName]

The names of the available joints in the observation.

enum JointName

The supported joint names for the body pose.

### Getting the joint name

func parentJointName(for: HumanBodyPose3DObservation.JointName) -> HumanBodyPose3DObservation.JointName

Returns the parent joint of the joint name you specify.

### Getting the camera position

func cameraRelativePosition(for: HumanBodyPose3DObservation.JointName) -> simd_float4x4

Returns a position relative to the camera for the body joint you specify.

### Getting the joint position

func pointInImage(for: HumanBodyPose3DObservation.JointName) -> NormalizedPoint

Returns a 2D point for the joint name you specify, relative to the input image.

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

