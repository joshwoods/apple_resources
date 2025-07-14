

- EventKit
- EKAlarm
-  structuredLocation 

Instance Property

# structuredLocation

The location to trigger an alarm.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.8+visionOS 1.0+watchOS 2.0+

``` source
@NSCopying
var structuredLocation: EKStructuredLocation? { get set }
```

## Discussion

This property is used in conjunction with proximity to perform geofence-based triggering of reminders.

## See Also

### Setting GeoFence-based Alarms

enum EKAlarmProximity

A value indicating whether an alarm is triggered by entering or exiting a region.

var proximity: EKAlarmProximity

A value indicating how a location-based alarm is triggered.

