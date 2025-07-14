

- Vision
- VNDetectTrajectoriesRequest
-  trajectoryLength 

Instance Property

# trajectoryLength

The number of points to detect before calculating a trajectory.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
var trajectoryLength: Int { get }
```

## See Also

### Configuring the Request

var targetFrameTime: CMTime

The requested target frame time for processing trajectory detection.

var objectMinimumNormalizedRadius: Float

The minimum radius of the bounding circle of the object to track.

var objectMaximumNormalizedRadius: Float

The maximum radius of the bounding circle of the object to track.

var minimumObjectSize: Float

The minimum radius of the tracked shape’s bounding circle.

Deprecated

var maximumObjectSize: Float

The maximum radius of the tracked shape’s bounding circle.

Deprecated

