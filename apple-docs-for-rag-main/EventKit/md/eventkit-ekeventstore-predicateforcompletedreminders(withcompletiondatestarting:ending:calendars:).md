

- EventKit
- EKEventStore
-  predicateForCompletedReminders(withCompletionDateStarting:ending:calendars:) 

Instance Method

# predicateForCompletedReminders(withCompletionDateStarting:ending:calendars:)

Creates a predicate to identify all completed reminders that occur within a given date range.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+visionOS 1.0+watchOS 2.0+

``` source
func predicateForCompletedReminders(
    withCompletionDateStarting startDate: Date?,
    ending endDate: Date?,
    calendars: [EKCalendar]?
) -> NSPredicate
```

## Parameters 

`startDate`  

The start date of the range of reminders fetched, or `nil` for all completed reminders before `endDate`.

`endDate`  

The end date of the range of reminders fetched, or `nil` for all completed reminders after `startDate`.

`calendars`  

An array of calendars to search.

## Return Value

A predicate to use when calling fetchReminders(matching:completion:).

## Mentioned in 

Retrieving events and reminders

## Discussion

Pass `nil` for both `startDate` and `endDate` to get all complete reminders in the specified calendars.

## See Also

### Searching calendars

func enumerateEvents(matching: NSPredicate, using: EKEventSearchCallback)

Finds all events that match a given predicate and calls a given callback for each event found.

func events(matching: NSPredicate) -> [EKEvent]

Finds all events that match a given predicate.

func fetchReminders(matching: NSPredicate, completion: ([EKReminder]?) -> Void) -> Any

Fetches reminders that match a given predicate.

func cancelFetchRequest(Any)

Cancels the request to fetch reminders.

func predicateForEvents(withStart: Date, end: Date, calendars: [EKCalendar]?) -> NSPredicate

Creates a predicate to identify events that occur within a given date range.

func predicateForReminders(in: [EKCalendar]?) -> NSPredicate

Creates a predicate to identify all reminders in a collection of calendars.

func predicateForIncompleteReminders(withDueDateStarting: Date?, ending: Date?, calendars: [EKCalendar]?) -> NSPredicate

Creates a predicate to identify all incomplete reminders that occur within a given date range.

typealias EKEventSearchCallback

The signature for a closure that operates on events when enumerating them.

