

- Core Motion
- CMPedometerData
-  currentPace 

Instance Property

# currentPace

The current pace of the user, measured in seconds per meter.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.15+watchOS 2.0+

``` source
var currentPace: NSNumber? { get }
```

## Discussion

During regular updates, this property is set to the user’s pace. The value in this property is `nil` when you are performing a query for historical pedometer data or when pace information is not yet available for the user. This property is also `nil` for devices that do not support the gathering of pace data.

## See Also

### Getting the Pedestrian Data

var numberOfSteps: NSNumber

The number of steps taken by the user.

var distance: NSNumber?

The estimated distance (in meters) traveled by the user.

var averageActivePace: NSNumber?

The average pace of the user, measured in seconds per meter.

var currentCadence: NSNumber?

The rate at which steps are taken, measured in steps per second.

