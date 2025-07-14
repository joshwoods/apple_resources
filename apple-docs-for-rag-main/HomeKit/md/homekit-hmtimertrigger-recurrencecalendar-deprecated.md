

- HomeKit
- HMTimerTrigger
-  recurrenceCalendar Deprecated

Instance Property

# recurrenceCalendar

The calendar in which the recurrence value is evaluated.

iOS 8.0–16.4DeprecatediPadOS 8.0–16.4DeprecatedMac Catalyst 8.0–16.4DeprecatedtvOS 10.0–16.4DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–9.4Deprecated

``` source
var recurrenceCalendar: Calendar? { get }
```

Deprecated

This property is no longer supported.

## Discussion

See recurrence for a discussion of how the recurrence value and recurrence calendar are used.

## See Also

### Deprecated symbols

init(name: String, fireDate: Date, timeZone: TimeZone?, recurrence: DateComponents?, recurrenceCalendar: Calendar?)

Initializes a timer trigger with specified timing information.

Deprecated

var timeZone: TimeZone?

The timezone in which to evaluate the fire time.

Deprecated

func updateTimeZone(TimeZone?, completionHandler: ((any Error)?) -> Void)

Updates the trigger’s time zone.

Deprecated

