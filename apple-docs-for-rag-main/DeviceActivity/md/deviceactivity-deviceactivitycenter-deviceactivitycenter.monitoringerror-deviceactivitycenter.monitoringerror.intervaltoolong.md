

- DeviceActivity
- DeviceActivityCenter
- DeviceActivityCenter.MonitoringError
-  DeviceActivityCenter.MonitoringError.intervalTooLong 

Case

# DeviceActivityCenter.MonitoringError.intervalTooLong

The activity’s schedule has an interval that is too long.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
case intervalTooLong
```

## Discussion

The maximum interval length for monitoring device activity events is one week.

## See Also

### Checking for Errors

case excessiveActivities

The calling process is monitoring too many activities.

case intervalTooShort

The activity’s schedule has an interval that is too short.

case invalidDateComponents

The schedule’s date range is invalid.

case unauthorized

The calling process isn’t authorized to monitor device activity.

