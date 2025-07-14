

- HomeKit
- HMTimerTrigger
-  timeZone Deprecated

Instance Property

# timeZone

The timezone in which to evaluate the fire time.

iOS 8.0–16.4DeprecatediPadOS 8.0–16.4DeprecatedMac Catalyst 8.0–16.4DeprecatedtvOS 10.0–16.4DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–9.4Deprecated

``` source
var timeZone: TimeZone? { get }
```

Deprecated

Use HMEventTrigger with HMCalendarEvent for triggers based on a time-zone-relative time of day.

## Discussion

If this value is `nil`, the trigger’s fire time will stay at the same relative time if the user changes timezones. If this value is set to a specific value, the trigger’s fire time will always be the same absolute time as evaluated in that time zone. A common value to set this to is the time zone where the accessories are physically located. This will result in the trigger firing at a specific time of day in that location, regardless of where the iOS device is located.

## See Also

### Deprecated symbols

init(name: String, fireDate: Date, timeZone: TimeZone?, recurrence: DateComponents?, recurrenceCalendar: Calendar?)

Initializes a timer trigger with specified timing information.

Deprecated

func updateTimeZone(TimeZone?, completionHandler: ((any Error)?) -> Void)

Updates the trigger’s time zone.

Deprecated

var recurrenceCalendar: Calendar?

The calendar in which the recurrence value is evaluated.

Deprecated

