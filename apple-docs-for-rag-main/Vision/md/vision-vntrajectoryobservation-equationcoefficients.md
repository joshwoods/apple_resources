

- Vision
- VNTrajectoryObservation
-  equationCoefficients 

Instance Property

# equationCoefficients

The coefficients of the parabolic equation.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
var equationCoefficients: simd_float3 { get }
```

## Discussion

This equation describes the parabola on which the detected contour is traveling. The equation and the projected points get refined over time.

## See Also

### Evaluating an Observation

var detectedPoints: [VNPoint]

The centroid points of the detected contour along the trajectory.

var projectedPoints: [VNPoint]

The centroids of the calculated trajectory from the detected points.

var movingAverageRadius: CGFloat

The moving average radius of the object the request is tracking.

