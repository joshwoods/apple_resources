

- Core Motion
- CMPedometerData
-  currentCadence 

Instance Property

# currentCadence

The rate at which steps are taken, measured in steps per second.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.15+watchOS 2.0+

``` source
var currentCadence: NSNumber? { get }
```

## Discussion

During regular updates, this property is set to the user’s cadence. The value in this property is `nil` when you are performing a query for historical pedometer data or when cadence information is not yet available for the user. This property is also `nil` for devices that do not support the gathering of cadence data.

## See Also

### Getting the Pedestrian Data

var numberOfSteps: NSNumber

The number of steps taken by the user.

var distance: NSNumber?

The estimated distance (in meters) traveled by the user.

var averageActivePace: NSNumber?

The average pace of the user, measured in seconds per meter.

var currentPace: NSNumber?

The current pace of the user, measured in seconds per meter.

