

- ARKit
- ObjectTrackingProvider
- ObjectTrackingProvider.TrackingConfiguration
-  stationaryObjectTrackingRate 

Instance Property

# stationaryObjectTrackingRate

The frequency at which object tracking runs for stationary objects, in Hz.

visionOS 2.0+

``` source
var stationaryObjectTrackingRate: Float
```

## Discussion

The framework clamps this to between `0` and `30` Hz.

## See Also

### Inspecting a tracking configuration

var detectionRate: Float

The frequency at which object detection runs, in Hz.

var maximumInstancesPerReferenceObject: Int

The maximum number of instances of each reference object type to allow tracking at once.

var maximumTrackableInstances: Int

The total number of object instances that you can track at the same time.

var movingObjectTrackingRate: Float

The frequency at which object tracking runs for moving objects, in Hz.

