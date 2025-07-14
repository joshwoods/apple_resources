

- EventKit
- EKEventStore
-  calendars Deprecated

Instance Property

# calendars

The calendars associated with the event store.

watchOS 2.0–2.0Deprecated

``` source
var calendars: [EKCalendar] { get }
```

Deprecated

Use calendars(for:) instead.

## Mentioned in 

Creating events and reminders

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

func saveCalendar(EKCalendar, commit: Bool) throws

Saves a calendar to the event store by either committing or batching the changes.

func removeCalendar(EKCalendar, commit: Bool) throws

Removes a calendar from the event store by either committing or batching the changes.

