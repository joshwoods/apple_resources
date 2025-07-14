

- DeviceActivity
- DeviceActivityCenter
- DeviceActivityCenter.MonitoringError
-  DeviceActivityCenter.MonitoringError.intervalTooShort 

Case

# DeviceActivityCenter.MonitoringError.intervalTooShort

The activity’s schedule has an interval that is too short.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
case intervalTooShort
```

## Discussion

The minimum interval length for monitoring device activity is fifteen minutes.

## See Also

### Checking for Errors

case excessiveActivities

The calling process is monitoring too many activities.

case intervalTooLong

The activity’s schedule has an interval that is too long.

case invalidDateComponents

The schedule’s date range is invalid.

case unauthorized

The calling process isn’t authorized to monitor device activity.

