

- Core Motion
- CMPedometerData
-  distance 

Instance Property

# distance

The estimated distance (in meters) traveled by the user.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.15+watchOS 2.0+

``` source
var distance: NSNumber? { get }
```

## Discussion

This value reflects the distance traveled while walking and running. The value in this property may be `nil` if distance estimation is not supported on the current device.

## See Also

### Getting the Pedestrian Data

var numberOfSteps: NSNumber

The number of steps taken by the user.

var averageActivePace: NSNumber?

The average pace of the user, measured in seconds per meter.

var currentPace: NSNumber?

The current pace of the user, measured in seconds per meter.

var currentCadence: NSNumber?

The rate at which steps are taken, measured in steps per second.

