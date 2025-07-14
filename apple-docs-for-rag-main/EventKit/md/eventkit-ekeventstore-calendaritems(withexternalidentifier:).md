

- EventKit
- EKEventStore
-  calendarItems(withExternalIdentifier:) 

Instance Method

# calendarItems(withExternalIdentifier:)

Locates all reminders or the first occurrences of all events with the specified external identifier.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+visionOS 1.0+watchOS 2.0+

``` source
func calendarItems(withExternalIdentifier externalIdentifier: String) -> [EKCalendarItem]
```

## Parameters 

`externalIdentifier`  

The calendar item’s external identifier.

## Return Value

An array of calendar items with the specified identifier.

## Discussion

Use calendarItemExternalIdentifier to obtain the external identifier. There may be more than one matching calendar item due to reasons discussed in `calendarItemExternalIdentifier`.

## See Also

### Accessing calendar events

func event(withIdentifier: String) -> EKEvent?

Locates the first occurrence of an event with a given identifier.

func calendarItem(withIdentifier: String) -> EKCalendarItem?

Locates a reminder or the first occurrence of an event with the specified identifier.

func remove(EKEvent, span: EKSpan) throws

Removes an event from the event store.

func remove(EKEvent, span: EKSpan, commit: Bool) throws

Removes an event or recurring events from the event store by either committing or batching the changes.

func remove(EKReminder, commit: Bool) throws

Removes a reminder from the event store by either committing or batching the changes.

func save(EKEvent, span: EKSpan) throws

Saves changes to an event permanently.

func save(EKEvent, span: EKSpan, commit: Bool) throws

Saves an event or recurring events to the event store by either committing or batching the changes.

func save(EKReminder, commit: Bool) throws

Saves changes to a reminder by either committing or batching the changes.

