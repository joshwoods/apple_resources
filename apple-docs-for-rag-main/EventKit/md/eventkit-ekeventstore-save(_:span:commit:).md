

- EventKit
- EKEventStore
-  save(\_:span:commit:) 

Instance Method

# save(\_:span:commit:)

Saves an event or recurring events to the event store by either committing or batching the changes.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.8+visionOS 1.0+

``` source
func save(
    _ event: EKEvent,
    span: EKSpan,
    commit: Bool
) throws
```

## Parameters 

`event`  

The event to save.

`span`  

The span that indicates whether to remove a single event or all future instances of the event in the case of a recurring event.

`commit`  

To save the event immediately, pass true; otherwise, the change is batched until the commit() method is invoked.

## Mentioned in 

Creating events and reminders

## Discussion

This method raises an exception if it’s passed an event from another event store.

When saving an event, it’s updated in the Calendar database. Any fields you didn’t modify are updated to reflect the most recent value in the database. If the event has been deleted from the database, it’s recreated as a new event.

Handling Errors in Swift

In Swift, this method returns `Void` and is marked with the `throws` keyword to indicate that it throws an error in cases of failure. Call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Related Documentation

func commit() throws

Commits all unsaved changes to the event store.

### Accessing calendar events

func event(withIdentifier: String) -> EKEvent?

Locates the first occurrence of an event with a given identifier.

func calendarItem(withIdentifier: String) -> EKCalendarItem?

Locates a reminder or the first occurrence of an event with the specified identifier.

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

func save(EKReminder, commit: Bool) throws

Saves changes to a reminder by either committing or batching the changes.

