

- EventKit
-  EKRecurrenceDayOfWeek 

Class

# EKRecurrenceDayOfWeek

A class that represents the day of the week.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.8+visionOS 1.0+watchOS 2.0+

``` source
class EKRecurrenceDayOfWeek
```

## Mentioned in 

Creating a recurring event

## Overview

The `EKRecurrenceDayOfWeek` class represents a day of the week for use with an EKRecurrenceRule object.

A day of the week can optionally have a week number, indicating a specific day in the recurrence rule’s frequency. For example, a day of the week with a day value of Tuesday and a week number of 2 would represent the second Tuesday of every month in a monthly recurrence rule, and the second Tuesday of every year in a yearly recurrence rule. A day of the week with a week number of 0 ignores its week number.

## Topics

### Creating a Day of the Week

enum EKWeekday

The day of the week.

convenience init(EKWeekday)

Creates and returns a day of the week with a given day.

convenience init(EKWeekday, weekNumber: Int)

Creates and returns an autoreleased day of the week with a given day and week number.

init(dayOfTheWeek: EKWeekday, weekNumber: Int)

Initializes and returns a day of the week with a given day and week number.

### Accessing Properties of a Day of the Week

var dayOfTheWeek: EKWeekday

The day of the week.

var weekNumber: Int

The week number of the day of the week.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Recurrence

Creating a recurring event

Set up an event or reminder that repeats.

class EKRecurrenceEnd

A class that defines the end of a recurrence rule.

class EKRecurrenceRule

A class that describes the pattern for a recurring event.

