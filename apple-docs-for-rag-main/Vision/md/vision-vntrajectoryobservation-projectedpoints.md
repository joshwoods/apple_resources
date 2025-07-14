

- Vision
- VNTrajectoryObservation
-  projectedPoints 

Instance Property

# projectedPoints

The centroids of the calculated trajectory from the detected points.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
var projectedPoints: [VNPoint] { get }
```

## Discussion

The projected points define the ideal trajectory described by the parabolic equation. The equation’s coefficients and the projected points of the detected trajectory get refined over time. The system limits the maximum number of cached points to the maximum points needed to describe the trajectory together with the parabolic equation.

## See Also

### Evaluating an Observation

var detectedPoints: [VNPoint]

The centroid points of the detected contour along the trajectory.

var equationCoefficients: simd_float3

The coefficients of the parabolic equation.

var movingAverageRadius: CGFloat

The moving average radius of the object the request is tracking.

