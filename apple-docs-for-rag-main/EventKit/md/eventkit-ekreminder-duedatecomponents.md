

- EventKit
- EKReminder
-  dueDateComponents 

Instance Property

# dueDateComponents

The date by which the reminder should be completed.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+visionOS 1.0+watchOS 2.0+

``` source
var dueDateComponents: DateComponents? { get set }
```

## Mentioned in 

Creating events and reminders

## Discussion

The use of date components allows the due date and its time zone to be represented in a single property. A `nil` time zone represents a floating date. Setting a date component without an hour, minute and second component will set the reminder to be an all-day reminder. If this property is set, the calendar must be set to `NSGregorianCalendar`; otherwise an exception is raised.

This components’s `timeZone` property is independent of time zone properties on startDateComponents and its super EKCalendarItem object. By default, the due date is set to the system time zone.

### Special Considerations

On iOS, Event Kit requires that a start date is set if the due date is set, however this is not a requirement in macOS.

## See Also

### Accessing Reminder Properties

enum EKReminderPriority

The priority of the reminder.

var priority: Int

The reminder’s priority.

var startDateComponents: DateComponents?

The start date of the task.

var isCompleted: Bool

A Boolean value determining whether or not the reminder is marked completed.

var completionDate: Date?

The date on which the reminder was completed.

