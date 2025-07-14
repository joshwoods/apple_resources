

- EventKit
- EKReminder
-  completionDate 

Instance Property

# completionDate

The date on which the reminder was completed.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+visionOS 1.0+watchOS 2.0+

``` source
var completionDate: Date? { get set }
```

## Mentioned in 

Creating events and reminders

## Discussion

Setting this property to a date will set isCompleted to true; setting this property to `nil` will set `completed` to false.

## See Also

### Accessing Reminder Properties

enum EKReminderPriority

The priority of the reminder.

var priority: Int

The reminder’s priority.

var startDateComponents: DateComponents?

The start date of the task.

var dueDateComponents: DateComponents?

The date by which the reminder should be completed.

var isCompleted: Bool

A Boolean value determining whether or not the reminder is marked completed.

