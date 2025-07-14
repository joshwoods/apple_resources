

- EventKit
- EKReminder
-  startDateComponents 

Instance Property

# startDateComponents

The start date of the task.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+visionOS 1.0+watchOS 2.0+

``` source
var startDateComponents: DateComponents? { get set }
```

## Mentioned in 

Creating events and reminders

## Discussion

The use of date components allows the start date and its time zone to be represented in a single property. A `nil` time zone represents a floating date. Setting a date component without an hour, minute and second component will set the reminder to be an all-day reminder. If this property is set, the calendar must be set to `NSGregorianCalendar`; otherwise an exception is raised.

The start date components’s `timeZone` property corresponds to the timeZone property on `EKCalendarItem`. A change in one value will cause a change in the other. Setting the time zone directly on the components does not guarantee that your changes will be saved; instead, pull this property from the reminder, set the time zone on it, and assign it back to the reminder:

```
NSDateComponents *start = myEKReminder.startDateComponents;
start.timeZone = myNSTimeZone;
myEKReminder.startDateComponents = start;
```

## See Also

### Accessing Reminder Properties

enum EKReminderPriority

The priority of the reminder.

var priority: Int

The reminder’s priority.

var dueDateComponents: DateComponents?

The date by which the reminder should be completed.

var isCompleted: Bool

A Boolean value determining whether or not the reminder is marked completed.

var completionDate: Date?

The date on which the reminder was completed.

