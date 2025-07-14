

- Vision
- DetectTrajectoriesRequest
-  objectMinimumNormalizedRadius 

Instance Property

# objectMinimumNormalizedRadius

The minimum radius of the bounding circle of the object to track.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
final var objectMinimumNormalizedRadius: Float { get set }
```

## See Also

### Inspecting a request

var objectMaximumNormalizedRadius: Float

The maximum radius of the bounding circle of the object to track.

var targetFrameTime: CMTime

The requested target frame time for processing trajectory detection.

let trajectoryLength: Int

The number of points to detect before calculating a trajectory.

