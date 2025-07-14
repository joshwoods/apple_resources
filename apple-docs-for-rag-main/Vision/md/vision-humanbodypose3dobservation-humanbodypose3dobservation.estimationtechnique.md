

- Vision
- HumanBodyPose3DObservation
-  HumanBodyPose3DObservation.EstimationTechnique 

Enumeration

# HumanBodyPose3DObservation.EstimationTechnique

Constants that identify body height estimation techniques.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
enum EstimationTechnique
```

## Topics

### Getting estimation techniques

case measured

A technique that uses LiDAR depth data to measure body height, in meters.

case reference

A technique that uses a reference height.

## Relationships

### Conforms To

- Decodable
- Encodable
- Equatable
- Hashable
- Sendable

## See Also

### Inspecting an observation

enum RequestDescriptor

A type that describes the request and revision combination.

let bodyHeight: Measurement&lt;UnitLength>

The estimated human body height, in meters.

let cameraOriginMatrix: simd_float4x4

A transform from the skeleton hip to the camera.

let heightEstimationTechnique: HumanBodyPose3DObservation.EstimationTechnique

The technique the framework uses to estimate body height.

