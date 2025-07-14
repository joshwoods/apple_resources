

- HomeKit
- HMTimerTrigger
-  updateTimeZone(\_:completionHandler:) Deprecated

Instance Method

# updateTimeZone(\_:completionHandler:)

Updates the trigger’s time zone.

iOS 8.0–16.4DeprecatediPadOS 8.0–16.4DeprecatedMac Catalyst 8.0–16.4DeprecatedtvOS 12.0–16.4DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 5.0–9.4Deprecated

``` source
func updateTimeZone(
    _ timeZone: TimeZone?,
    completionHandler completion: @escaping ((any Error)?) -> Void
)
```

``` source
func updateTimeZone(_ timeZone: TimeZone?) async throws
```

Deprecated

Use HMEventTrigger with HMCalendarEvent for triggers based on a time-zone-relative time of day.

## Parameters 

`timeZone`  

The new time zone; may be `nil`.

`completion`  

The block executed after the request is processed.

error  
`nil` on success; otherwise, error object indicating the reason for failure.

## Discussion

See timeZone for a description of how the time zone is interpreted.

## See Also

### Deprecated symbols

init(name: String, fireDate: Date, timeZone: TimeZone?, recurrence: DateComponents?, recurrenceCalendar: Calendar?)

Initializes a timer trigger with specified timing information.

Deprecated

var timeZone: TimeZone?

The timezone in which to evaluate the fire time.

Deprecated

var recurrenceCalendar: Calendar?

The calendar in which the recurrence value is evaluated.

Deprecated

