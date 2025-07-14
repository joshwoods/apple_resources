

- EventKit
- EKReminder
-  isCompleted 

Instance Property

# isCompleted

A Boolean value determining whether or not the reminder is marked completed.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+visionOS 1.0+watchOS 2.0+

``` source
var isCompleted: Bool { get set }
```

## Discussion

Setting this property to true will set completionDate to the current date; setting this property to false will set `completionDate` to `nil`.

### Special Considerations

If the reminder was completed using a different client, you may encounter the case where this property is true, but `completionDate` is `nil`.

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

var completionDate: Date?

The date on which the reminder was completed.

