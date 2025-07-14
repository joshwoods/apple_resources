

- DeviceActivity
- DeviceActivityCenter
- DeviceActivityCenter.MonitoringError
-  DeviceActivityCenter.MonitoringError.excessiveActivities 

Case

# DeviceActivityCenter.MonitoringError.excessiveActivities

The calling process is monitoring too many activities.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
case excessiveActivities
```

## Discussion

The maximum number of activities that can be monitored at one time by an app and its extensions is twenty.

## See Also

### Checking for Errors

case intervalTooLong

The activity’s schedule has an interval that is too long.

case intervalTooShort

The activity’s schedule has an interval that is too short.

case invalidDateComponents

The schedule’s date range is invalid.

case unauthorized

The calling process isn’t authorized to monitor device activity.

