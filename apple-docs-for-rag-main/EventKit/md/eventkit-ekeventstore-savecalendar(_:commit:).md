

- EventKit
- EKEventStore
-  saveCalendar(\_:commit:) 

Instance Method

# saveCalendar(\_:commit:)

Saves a calendar to the event store by either committing or batching the changes.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.8+visionOS 1.0+

``` source
func saveCalendar(
    _ calendar: EKCalendar,
    commit: Bool
) throws
```

## Parameters 

`calendar`  

The calendar to save.

`commit`  

true to save the calendar immediately; otherwise, the change is batched until the commit() method is invoked.

## Discussion

This method raises an exception if `calendar` belongs to another event store.

Handling Errors in Swift

In Swift, this method returns `Void` and is marked with the `throws` keyword to indicate that it throws an error in cases of failure. Call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Accessing calendars

var defaultCalendarForNewEvents: EKCalendar?

The calendar that events are added to by default, as specified by user settings.

func defaultCalendarForNewReminders() -> EKCalendar?

Identifies the default calendar for adding reminders to, as specified by user settings.

func calendars(for: EKEntityType) -> [EKCalendar]

Identifies the calendars that support a given entity type, such as reminders or events.

func calendar(withIdentifier: String) -> EKCalendar?

Locates a calendar with the specified identifier.

func removeCalendar(EKCalendar, commit: Bool) throws

Removes a calendar from the event store by either committing or batching the changes.

var calendars: [EKCalendar]

The calendars associated with the event store.

Deprecated

