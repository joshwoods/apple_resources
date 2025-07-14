

- EventKit
- EKCalendarItem
-  removeAlarm(\_:) 

Instance Method

# removeAlarm(\_:)

Removes an alarm from the calendar item.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.8+visionOS 1.0+watchOS 2.0+

``` source
func removeAlarm(_ alarm: EKAlarm)
```

## Parameters 

`alarm`  

The alarm to be removed.

## Mentioned in 

Setting an alarm

## See Also

### Adding and Removing Alarms

var hasAlarms: Bool

A Boolean value that indicates whether the calendar item has alarms.

func addAlarm(EKAlarm)

Adds an alarm to the receiver.

var alarms: [EKAlarm]?

The alarms associated with the calendar item, as an array of EKAlarm objects.

