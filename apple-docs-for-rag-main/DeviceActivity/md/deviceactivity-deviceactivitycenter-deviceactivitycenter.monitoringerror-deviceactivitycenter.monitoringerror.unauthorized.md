

- DeviceActivity
- DeviceActivityCenter
- DeviceActivityCenter.MonitoringError
-  DeviceActivityCenter.MonitoringError.unauthorized 

Case

# DeviceActivityCenter.MonitoringError.unauthorized

The calling process isn’t authorized to monitor device activity.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
case unauthorized
```

## Discussion

See the `FamilyControls` framework for more details about authorization to access the user’s device activity.

## See Also

### Checking for Errors

case excessiveActivities

The calling process is monitoring too many activities.

case intervalTooLong

The activity’s schedule has an interval that is too long.

case intervalTooShort

The activity’s schedule has an interval that is too short.

case invalidDateComponents

The schedule’s date range is invalid.

