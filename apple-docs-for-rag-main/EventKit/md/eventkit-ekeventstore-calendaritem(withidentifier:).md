

- EventKit
- EKEventStore
-  calendarItem(withIdentifier:) 

Instance Method

# calendarItem(withIdentifier:)

Locates a reminder or the first occurrence of an event with the specified identifier.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+visionOS 1.0+watchOS 2.0+

``` source
func calendarItem(withIdentifier identifier: String) -> EKCalendarItem?
```

## Parameters 

`identifier`  

The calendar item’s unique identifier.

## Return Value

The reminder or the first occurrence of an event with the specified identifier, or `nil` if neither is found.

## Mentioned in 

Retrieving events and reminders

## See Also

### Accessing calendar events

func event(withIdentifier: String) -> EKEvent?

Locates the first occurrence of an event with a given identifier.

func calendarItems(withExternalIdentifier: String) -> [EKCalendarItem]

Locates all reminders or the first occurrences of all events with the specified external identifier.

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

