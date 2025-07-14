

- Vision
- TrajectoryObservation
-  movingAverageRadius 

Instance Property

# movingAverageRadius

The moving average radius of the object the request is tracking.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
let movingAverageRadius: CGFloat
```

## See Also

### Inspecting an observation

let detectedPoints: [NormalizedPoint]

The centroid points of the detected contour along the trajectory.

let projectedPoints: [NormalizedPoint]

The centroids of the calculated trajectory from the detected points.

let equationCoefficients: simd_float3

The coefficients of the parabolic equation.

