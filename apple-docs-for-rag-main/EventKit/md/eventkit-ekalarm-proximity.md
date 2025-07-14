

- EventKit
- EKAlarm
-  proximity 

Instance Property

# proximity

A value indicating how a location-based alarm is triggered.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.8+visionOS 1.0+watchOS 2.0+

``` source
var proximity: EKAlarmProximity { get set }
```

## Discussion

Alarms can be set to trigger when entering or exiting a location specified by structuredLocation. By default, alarms are not affected by location.

## See Also

### Setting GeoFence-based Alarms

enum EKAlarmProximity

A value indicating whether an alarm is triggered by entering or exiting a region.

var structuredLocation: EKStructuredLocation?

The location to trigger an alarm.

