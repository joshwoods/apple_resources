

- Vision
- VNHumanBodyPose3DObservation
-  VNHumanBodyPose3DObservation.HeightEstimation 

Enumeration

# VNHumanBodyPose3DObservation.HeightEstimation

Constants that identify body height estimation techniques.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.0+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
enum HeightEstimation
```

## Topics

### Techniques

case measured

A technique that uses LiDAR depth data to measure body height, in meters.

case reference

A technique that uses a reference height.

case measured

A technique that uses LiDAR depth data to measure body height, in meters.

case reference

A technique that uses a reference height.

### Creating a Technique

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Getting the Body Height

var heightEstimation: VNHumanBodyPose3DObservation.HeightEstimation

The technique the framework uses to estimate body height.

var bodyHeight: Float

The estimated human body height, in meters.

