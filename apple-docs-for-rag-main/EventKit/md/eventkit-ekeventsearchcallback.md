

- EventKit
-  EKEventSearchCallback 

Type Alias

# EKEventSearchCallback

The signature for a closure that operates on events when enumerating them.

iOSiPadOSMac CatalystmacOSvisionOSwatchOS

``` source
typealias EKEventSearchCallback = (EKEvent, UnsafeMutablePointer) -> Void
```

## Parameters 

`event`  

An event object to operate on.

`stop`  

A pointer to a Boolean value. Set this value to true to stop enumerating events.

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

func predicateForCompletedReminders(withCompletionDateStarting: Date?, ending: Date?, calendars: [EKCalendar]?) -> NSPredicate

Creates a predicate to identify all completed reminders that occur within a given date range.

func predicateForIncompleteReminders(withDueDateStarting: Date?, ending: Date?, calendars: [EKCalendar]?) -> NSPredicate

Creates a predicate to identify all incomplete reminders that occur within a given date range.

