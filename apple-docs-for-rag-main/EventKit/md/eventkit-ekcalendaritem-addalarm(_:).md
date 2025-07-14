

- EventKit
- EKCalendarItem
-  addAlarm(\_:) 

Instance Method

# addAlarm(\_:)

Adds an alarm to the receiver.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.8+visionOS 1.0+watchOS 2.0+

``` source
func addAlarm(_ alarm: EKAlarm)
```

## Parameters 

`alarm`  

The alarm to be added.

## Mentioned in 

Creating events and reminders

Setting an alarm

## See Also

### Adding and Removing Alarms

var hasAlarms: Bool

A Boolean value that indicates whether the calendar item has alarms.

func removeAlarm(EKAlarm)

Removes an alarm from the calendar item.

var alarms: [EKAlarm]?

The alarms associated with the calendar item, as an array of EKAlarm objects.

