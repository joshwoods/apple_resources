

- EventKit
- EKEventStore
-  cancelFetchRequest(\_:) 

Instance Method

# cancelFetchRequest(\_:)

Cancels the request to fetch reminders.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+visionOS 1.0+watchOS 2.0+

``` source
func cancelFetchRequest(_ fetchIdentifier: Any)
```

## Parameters 

`fetchIdentifier`  

The identifier of the request as returned by fetchReminders(matching:completion:).

## Mentioned in 

Retrieving events and reminders

## Discussion

After canceling a fetch request, EventKit doesn’t call the completion originally specified in fetchReminders(matching:completion:).

## See Also

### Searching calendars

func enumerateEvents(matching: NSPredicate, using: EKEventSearchCallback)

Finds all events that match a given predicate and calls a given callback for each event found.

func events(matching: NSPredicate) -> [EKEvent]

Finds all events that match a given predicate.

func fetchReminders(matching: NSPredicate, completion: ([EKReminder]?) -> Void) -> Any

Fetches reminders that match a given predicate.

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

