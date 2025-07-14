

- EventKit
- EKEventStore
-  fetchReminders(matching:completion:) 

Instance Method

# fetchReminders(matching:completion:)

Fetches reminders that match a given predicate.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+visionOS 1.0+watchOS 2.0+

``` source
func fetchReminders(
    matching predicate: NSPredicate,
    completion: @escaping ([EKReminder]?) -> Void
) -> Any
```

## Parameters 

`predicate`  

A search predicate created with predicateForReminders(in:).

`completion`  

A closure that receives the reminders that match `predicate`.

## Return Value

A value that represents the asynchronous fetch request. To cancel a fetch request before it completes, pass this value to cancelFetchRequest(_:).

## Mentioned in 

Retrieving events and reminders

## Discussion

Only committed reminders are included in the results. To include reminders saved using save(_:commit:) with the `commit` parameter set to false, call commit() first.

This method fetches reminders asynchronously.

## See Also

### Searching calendars

func enumerateEvents(matching: NSPredicate, using: EKEventSearchCallback)

Finds all events that match a given predicate and calls a given callback for each event found.

func events(matching: NSPredicate) -> [EKEvent]

Finds all events that match a given predicate.

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

