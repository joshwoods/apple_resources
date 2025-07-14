

- Vision
- TrajectoryObservation
-  detectedPoints 

Instance Property

# detectedPoints

The centroid points of the detected contour along the trajectory.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
let detectedPoints: [NormalizedPoint]
```

## Discussion

The detected points may differ slightly from the ideal trajectory because they fall within the allowed tolerance. The system limits the maximum number of points based on the maximum trajectory length set in the request.

## See Also

### Inspecting an observation

let projectedPoints: [NormalizedPoint]

The centroids of the calculated trajectory from the detected points.

let equationCoefficients: simd_float3

The coefficients of the parabolic equation.

let movingAverageRadius: CGFloat

The moving average radius of the object the request is tracking.

