

- EventKit
- EKEventStore
-  remove(\_:span:) 

Instance Method

# remove(\_:span:)

Removes an event from the event store.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.14+visionOS 1.0+

``` source
func remove(
    _ event: EKEvent,
    span: EKSpan
) throws
```

## Parameters 

`event`  

The event to remove.

`span`  

The span that indicates whether to remove a single event or all future instances of the event in the case of a recurring event.

## Discussion

This method raises an exception if the event belongs to another event store.

Handling Errors in Swift

In Swift, this method returns `Void` and is marked with the `throws` keyword to indicate that it throws an error in cases of failure. Call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Accessing calendar events

func event(withIdentifier: String) -> EKEvent?

Locates the first occurrence of an event with a given identifier.

func calendarItem(withIdentifier: String) -> EKCalendarItem?

Locates a reminder or the first occurrence of an event with the specified identifier.

func calendarItems(withExternalIdentifier: String) -> [EKCalendarItem]

Locates all reminders or the first occurrences of all events with the specified external identifier.

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

