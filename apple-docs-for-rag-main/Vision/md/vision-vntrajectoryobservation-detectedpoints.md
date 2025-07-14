

- Vision
- VNTrajectoryObservation
-  detectedPoints 

Instance Property

# detectedPoints

The centroid points of the detected contour along the trajectory.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
var detectedPoints: [VNPoint] { get }
```

## Discussion

The detected points may differ slightly from the ideal trajectory because they fall within the allowed tolerance. The system limits the maximum number of points based on the maximum trajectory length set in the request.

## See Also

### Evaluating an Observation

var projectedPoints: [VNPoint]

The centroids of the calculated trajectory from the detected points.

var equationCoefficients: simd_float3

The coefficients of the parabolic equation.

var movingAverageRadius: CGFloat

The moving average radius of the object the request is tracking.

