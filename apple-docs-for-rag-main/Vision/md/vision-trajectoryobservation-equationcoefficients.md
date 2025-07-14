

- Vision
- TrajectoryObservation
-  equationCoefficients 

Instance Property

# equationCoefficients

The coefficients of the parabolic equation.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
let equationCoefficients: simd_float3
```

## Discussion

This equation describes the parabola on which the detected contour is traveling. The equation and the projected points get refined over time.

## See Also

### Inspecting an observation

let detectedPoints: [NormalizedPoint]

The centroid points of the detected contour along the trajectory.

let projectedPoints: [NormalizedPoint]

The centroids of the calculated trajectory from the detected points.

let movingAverageRadius: CGFloat

The moving average radius of the object the request is tracking.

