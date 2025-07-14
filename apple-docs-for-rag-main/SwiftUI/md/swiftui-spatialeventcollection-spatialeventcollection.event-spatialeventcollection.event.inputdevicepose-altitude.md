

- SwiftUI
- SpatialEventCollection
- SpatialEventCollection.Event
- SpatialEventCollection.Event.InputDevicePose
-  altitude 

Instance Property

# altitude

The altitude angle.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+watchOS 11.0+

``` source
var altitude: Angle
```

## Discussion

An angle of zero indicates that the device is parallel to the content, while 90 degrees indicates that it is normal to the content surface.

## See Also

### Getting the event type

var azimuth: Angle

The azimuth angle.

var pose3D: Pose3D

The 3D pose of the input device.

