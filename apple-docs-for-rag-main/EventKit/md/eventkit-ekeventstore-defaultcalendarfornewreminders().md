

- EventKit
- EKEventStore
-  defaultCalendarForNewReminders() 

Instance Method

# defaultCalendarForNewReminders()

Identifies the default calendar for adding reminders to, as specified by user settings.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+visionOS 1.0+watchOS 2.0+

``` source
func defaultCalendarForNewReminders() -> EKCalendar?
```

## Return Value

The calendar that reminders are added to by default.

## See Also

### Accessing calendars

var defaultCalendarForNewEvents: EKCalendar?

The calendar that events are added to by default, as specified by user settings.

func calendars(for: EKEntityType) -> [EKCalendar]

Identifies the calendars that support a given entity type, such as reminders or events.

func calendar(withIdentifier: String) -> EKCalendar?

Locates a calendar with the specified identifier.

func saveCalendar(EKCalendar, commit: Bool) throws

Saves a calendar to the event store by either committing or batching the changes.

func removeCalendar(EKCalendar, commit: Bool) throws

Removes a calendar from the event store by either committing or batching the changes.

var calendars: [EKCalendar]

The calendars associated with the event store.

Deprecated

