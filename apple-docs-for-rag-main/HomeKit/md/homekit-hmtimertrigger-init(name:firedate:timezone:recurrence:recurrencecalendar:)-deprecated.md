

- HomeKit
- HMTimerTrigger
-  init(name:fireDate:timeZone:recurrence:recurrenceCalendar:) Deprecated

Initializer

# init(name:fireDate:timeZone:recurrence:recurrenceCalendar:)

Initializes a timer trigger with specified timing information.

iOS 8.0–16.4DeprecatediPadOS 8.0–16.4DeprecatedMac Catalyst 8.0–16.4DeprecatedtvOS 10.0–16.4DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–9.4Deprecated

``` source
init(
    name: String,
    fireDate: Date,
    timeZone: TimeZone?,
    recurrence: DateComponents?,
    recurrenceCalendar: Calendar?
)
```

## Parameters 

`name`  

The name of the timer trigger.

`fireDate`  

The first fire date.

`timeZone`  

The time zone for the first fire date. Pass `nil` to use the default time zone. See timeZone for a description of how the time zone is interpreted.

`recurrence`  

The recurrence interval on which to fire the trigger. `nil` indicates a one-time trigger.

`recurrenceCalendar`  

The calendar in which to evaluate the recurrence interval of a timer trigger. May be `nil`, in which case the current calendar current is used.

## Return Value

A newly-initialized timer trigger with the specified values.

## Discussion

A new timer trigger starts out disabled, and must be enabled using enable(_:completionHandler:) before use.

## See Also

### Deprecated symbols

var timeZone: TimeZone?

The timezone in which to evaluate the fire time.

Deprecated

func updateTimeZone(TimeZone?, completionHandler: ((any Error)?) -> Void)

Updates the trigger’s time zone.

Deprecated

var recurrenceCalendar: Calendar?

The calendar in which the recurrence value is evaluated.

Deprecated

