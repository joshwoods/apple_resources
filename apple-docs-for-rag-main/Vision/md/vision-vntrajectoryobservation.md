

- Vision
-  VNTrajectoryObservation 

Class

# VNTrajectoryObservation

An observation that describes a detected trajectory.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
class VNTrajectoryObservation
```

## Mentioned in 

Identifying Trajectories in Video

## Topics

### Evaluating an Observation

var detectedPoints: [VNPoint]

The centroid points of the detected contour along the trajectory.

var projectedPoints: [VNPoint]

The centroids of the calculated trajectory from the detected points.

var equationCoefficients: simd_float3

The coefficients of the parabolic equation.

var movingAverageRadius: CGFloat

The moving average radius of the object the request is tracking.

## Relationships

### Inherits From

- VNObservation

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding
- VNRequestRevisionProviding

## See Also

### Inspecting the Results

var results: [VNTrajectoryObservation]?

The array of detected trajectory observations.

