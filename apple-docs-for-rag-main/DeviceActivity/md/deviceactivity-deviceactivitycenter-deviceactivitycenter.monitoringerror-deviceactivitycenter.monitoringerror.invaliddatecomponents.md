

- DeviceActivity
- DeviceActivityCenter
- DeviceActivityCenter.MonitoringError
-  DeviceActivityCenter.MonitoringError.invalidDateComponents 

Case

# DeviceActivityCenter.MonitoringError.invalidDateComponents

The schedule’s date range is invalid.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
case invalidDateComponents
```

## Discussion

The schedule’s start or end date components don’t match any future dates. Consider specifying a different calendar or different date components.

## See Also

### Checking for Errors

case excessiveActivities

The calling process is monitoring too many activities.

case intervalTooLong

The activity’s schedule has an interval that is too long.

case intervalTooShort

The activity’s schedule has an interval that is too short.

case unauthorized

The calling process isn’t authorized to monitor device activity.

