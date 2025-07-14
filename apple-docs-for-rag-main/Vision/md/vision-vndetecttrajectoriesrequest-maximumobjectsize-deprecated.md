

- Vision
- VNDetectTrajectoriesRequest
-  maximumObjectSize Deprecated

Instance Property

# maximumObjectSize

The maximum radius of the tracked shape’s bounding circle.

iOS 14.0–14.0DeprecatediPadOS 14.0–14.0DeprecatedMac Catalyst 14.0–14.0DeprecatedmacOS 11.0–11.0DeprecatedtvOS 14.0–14.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
var maximumObjectSize: Float { get set }
```

Deprecated

Use objectMaximumNormalizedRadius instead.

## Mentioned in 

Identifying Trajectories in Video

## Discussion

Set the maximum size to filter out unwanted trajectories from larger objects moving through the scene. The default value is 1.0, which means to apply no filtering.

Changing this property value from frame to frame can produce erratic trajectories because objects either disappear or are added to the tracking based on this filtering.

Specify the size in normalized (0.0 to 1.0) coordinates.

## See Also

### Configuring the Request

var targetFrameTime: CMTime

The requested target frame time for processing trajectory detection.

var trajectoryLength: Int

The number of points to detect before calculating a trajectory.

var objectMinimumNormalizedRadius: Float

The minimum radius of the bounding circle of the object to track.

var objectMaximumNormalizedRadius: Float

The maximum radius of the bounding circle of the object to track.

var minimumObjectSize: Float

The minimum radius of the tracked shape’s bounding circle.

Deprecated

