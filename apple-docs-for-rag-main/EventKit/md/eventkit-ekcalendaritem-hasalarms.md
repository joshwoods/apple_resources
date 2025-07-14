

- EventKit
- EKCalendarItem
-  hasAlarms 

Instance Property

# hasAlarms

A Boolean value that indicates whether the calendar item has alarms.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.8+visionOS 1.0+watchOS 2.0+

``` source
var hasAlarms: Bool { get }
```

## Discussion

If true, the calendar item has alarms; otherwise it does not.

## See Also

### Adding and Removing Alarms

func addAlarm(EKAlarm)

Adds an alarm to the receiver.

func removeAlarm(EKAlarm)

Removes an alarm from the calendar item.

var alarms: [EKAlarm]?

The alarms associated with the calendar item, as an array of EKAlarm objects.

