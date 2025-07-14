

- Vision
- VNTrajectoryObservation
-  movingAverageRadius 

Instance Property

# movingAverageRadius

The moving average radius of the object the request is tracking.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
var movingAverageRadius: CGFloat { get }
```

## See Also

### Evaluating an Observation

var detectedPoints: [VNPoint]

The centroid points of the detected contour along the trajectory.

var projectedPoints: [VNPoint]

The centroids of the calculated trajectory from the detected points.

var equationCoefficients: simd_float3

The coefficients of the parabolic equation.

