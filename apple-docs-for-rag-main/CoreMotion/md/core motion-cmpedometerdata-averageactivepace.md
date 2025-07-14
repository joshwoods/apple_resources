

- Core Motion
- CMPedometerData
-  averageActivePace 

Instance Property

# averageActivePace

The average pace of the user, measured in seconds per meter.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.15+watchOS 3.0+

``` source
var averageActivePace: NSNumber? { get }
```

## Discussion

During regular updates, this property is set to the user’s average active pace since startUpdates(from:withHandler:) was called. When you perform historical queries, the property is set to the average active pace between startDate and endDate.

The property averages the user’s pace only during periods of activity and it omits all periods of inactivity. The value of this property is `nil` when you are performing a query for historical pedometer data and the information is not available (such as when the user did not move between `startDate` and `endDate`). This property is also `nil` for devices that do not support the gathering of pace data.

## See Also

### Getting the Pedestrian Data

var numberOfSteps: NSNumber

The number of steps taken by the user.

var distance: NSNumber?

The estimated distance (in meters) traveled by the user.

var currentPace: NSNumber?

The current pace of the user, measured in seconds per meter.

var currentCadence: NSNumber?

The rate at which steps are taken, measured in steps per second.

