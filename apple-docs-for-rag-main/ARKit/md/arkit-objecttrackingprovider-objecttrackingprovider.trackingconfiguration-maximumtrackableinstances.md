

- ARKit
- ObjectTrackingProvider
- ObjectTrackingProvider.TrackingConfiguration
-  maximumTrackableInstances 

Instance Property

# maximumTrackableInstances

The total number of object instances that you can track at the same time.

visionOS 2.0+

``` source
var maximumTrackableInstances: Int
```

## See Also

### Inspecting a tracking configuration

var detectionRate: Float

The frequency at which object detection runs, in Hz.

var maximumInstancesPerReferenceObject: Int

The maximum number of instances of each reference object type to allow tracking at once.

var movingObjectTrackingRate: Float

The frequency at which object tracking runs for moving objects, in Hz.

var stationaryObjectTrackingRate: Float

The frequency at which object tracking runs for stationary objects, in Hz.

