

- EventKit
- EKCalendarItem
-  alarms 

Instance Property

# alarms

The alarms associated with the calendar item, as an array of EKAlarm objects.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.8+visionOS 1.0+watchOS 2.0+

``` source
var alarms: [EKAlarm]? { get set }
```

## Mentioned in 

Creating events and reminders

## Discussion

This property is `nil` if the calendar item has no alarms.

## See Also

### Adding and Removing Alarms

var hasAlarms: Bool

A Boolean value that indicates whether the calendar item has alarms.

func addAlarm(EKAlarm)

Adds an alarm to the receiver.

func removeAlarm(EKAlarm)

Removes an alarm from the calendar item.

