

- EventKit
-  EKReminder 

Class

# EKReminder

A class that represents a reminder in a calendar.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+visionOS 1.0+watchOS 2.0+

``` source
class EKReminder
```

## Mentioned in 

Creating events and reminders

## Overview

Use the init(eventStore:) method to create a new reminder. Use the properties in the class to get and modify certain information about a reminder.

## Topics

### Creating a Reminder

init(eventStore: EKEventStore)

Creates and returns a new reminder in the given event store.

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

var completionDate: Date?

The date on which the reminder was completed.

## Relationships

### Inherits From

- EKCalendarItem

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Events and reminders

Creating events and reminders

Create and modify events and reminders in a person’s database.

Retrieving events and reminders

Fetch events and reminders from the Calendar database.

Updating with notifications

Register for notifications about changes and keep your app up to date.

Managing Location-Based Reminders

Add, fetch, complete, remove, and sort location-based reminders in your app.

class EKEvent

A class that represents an event in a calendar.

