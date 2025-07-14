

- EventKit
-  EKReminderPriority 

Enumeration

# EKReminderPriority

The priority of the reminder.

iOSiPadOSMac CatalystmacOSvisionOSwatchOS

``` source
enum EKReminderPriority
```

## Topics

### Constants

case none

The reminder has no priority set.

case high

The reminder is high priority.

case medium

The reminder is medium priority.

case low

The reminder is low priority.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Accessing Reminder Properties

var priority: Int

The reminder’s priority.

var startDateComponents: DateComponents?

The start date of the task.

var dueDateComponents: DateComponents?

The date by which the reminder should be completed.

var isCompleted: Bool

A Boolean value determining whether or not the reminder is marked completed.

var completionDate: Date?

The date on which the reminder was completed.

