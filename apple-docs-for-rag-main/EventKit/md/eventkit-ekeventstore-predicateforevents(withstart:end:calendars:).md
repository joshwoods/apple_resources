

- EventKit
- EKEventStore
-  predicateForEvents(withStart:end:calendars:) 

Instance Method

# predicateForEvents(withStart:end:calendars:)

Creates a predicate to identify events that occur within a given date range.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.8+visionOS 1.0+watchOS 2.0+

``` source
func predicateForEvents(
    withStart startDate: Date,
    end endDate: Date,
    calendars: [EKCalendar]?
) -> NSPredicate
```

## Parameters 

`startDate`  

The start date of the range of events fetched.

`endDate`  

The end date of the range of events fetched.

`calendars`  

An array of calendars to search, or `nil` to search all calendars.

## Return Value

A predicate to use when calling enumerateEvents(matching:using:) or events(matching:).

## Mentioned in 

Retrieving events and reminders

## Discussion

Use this method to create a predicate for use with events(matching:) or enumerateEvents(matching:using:). The events returned using this predicate are in the default time zone. For performance reasons, this method matches only those events within a four-year time span. If the date range between `startDate` and `endDate` is greater than four years, it’s shortened to the first four years.

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

func predicateForReminders(in: [EKCalendar]?) -> NSPredicate

Creates a predicate to identify all reminders in a collection of calendars.

func predicateForCompletedReminders(withCompletionDateStarting: Date?, ending: Date?, calendars: [EKCalendar]?) -> NSPredicate

Creates a predicate to identify all completed reminders that occur within a given date range.

func predicateForIncompleteReminders(withDueDateStarting: Date?, ending: Date?, calendars: [EKCalendar]?) -> NSPredicate

Creates a predicate to identify all incomplete reminders that occur within a given date range.

typealias EKEventSearchCallback

The signature for a closure that operates on events when enumerating them.

