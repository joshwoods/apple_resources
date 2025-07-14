

- EventKit
- EKEventStore
-  events(matching:) 

Instance Method

# events(matching:)

Finds all events that match a given predicate.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.8+visionOS 1.0+watchOS 2.0+

``` source
func events(matching predicate: NSPredicate) -> [EKEvent]
```

## Parameters 

`predicate`  

A search predicate created with predicateForEvents(withStart:end:calendars:).

## Return Value

An array of events that match `predicate`.

## Mentioned in 

Retrieving events and reminders

## Discussion

Only committed events are included in the results. To include events saved using save(_:span:commit:) with the `commit` parameter set to false, call commit() first.

This method is synchronous. For asynchronous behavior, run the method on another thread with dispatch_async or Operation.

## See Also

### Searching calendars

func enumerateEvents(matching: NSPredicate, using: EKEventSearchCallback)

Finds all events that match a given predicate and calls a given callback for each event found.

func fetchReminders(matching: NSPredicate, completion: ([EKReminder]?) -> Void) -> Any

Fetches reminders that match a given predicate.

func cancelFetchRequest(Any)

Cancels the request to fetch reminders.

func predicateForEvents(withStart: Date, end: Date, calendars: [EKCalendar]?) -> NSPredicate

Creates a predicate to identify events that occur within a given date range.

func predicateForReminders(in: [EKCalendar]?) -> NSPredicate

Creates a predicate to identify all reminders in a collection of calendars.

func predicateForCompletedReminders(withCompletionDateStarting: Date?, ending: Date?, calendars: [EKCalendar]?) -> NSPredicate

Creates a predicate to identify all completed reminders that occur within a given date range.

func predicateForIncompleteReminders(withDueDateStarting: Date?, ending: Date?, calendars: [EKCalendar]?) -> NSPredicate

Creates a predicate to identify all incomplete reminders that occur within a given date range.

typealias EKEventSearchCallback

The signature for a closure that operates on events when enumerating them.

