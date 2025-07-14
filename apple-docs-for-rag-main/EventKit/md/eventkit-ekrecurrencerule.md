

- EventKit
-  EKRecurrenceRule 

Class

# EKRecurrenceRule

A class that describes the pattern for a recurring event.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.8+visionOS 1.0+watchOS 2.0+

``` source
class EKRecurrenceRule
```

## Mentioned in 

Creating a recurring event

## Overview

After you create a recurrence rule, assign it to an event with the method of EKEvent.

Recurrence rules can have an end, represented by an EKRecurrenceEnd object. The end can be based on a specific date or a maximum number of occurrences.

Note

It is currently not possible to directly modify an `EKRecurrenceRule` or any of its properties. This functionality is achieved by creating a new `EKRecurrenceRule` and setting an event or reminder to use the newly created rule.

## Topics

### Creating a Basic Recurrence Rule

enum EKSpan

An object that indicates whether modifications should apply to a single event or all future events of a recurring event.

init(recurrenceWith: EKRecurrenceFrequency, interval: Int, end: EKRecurrenceEnd?)

Initializes and returns a simple recurrence rule with a given frequency, interval, and end.

### Creating a Complex Recurrence Rule

init(recurrenceWith: EKRecurrenceFrequency, interval: Int, daysOfTheWeek: [EKRecurrenceDayOfWeek]?, daysOfTheMonth: [NSNumber]?, monthsOfTheYear: [NSNumber]?, weeksOfTheYear: [NSNumber]?, daysOfTheYear: [NSNumber]?, setPositions: [NSNumber]?, end: EKRecurrenceEnd?)

Initializes and returns a recurrence rule with a given frequency and additional scheduling information.

### Accessing Recurrence Rule Properties

enum EKRecurrenceFrequency

The frequency for recurrence rules.

var calendarIdentifier: String

The identifier for the recurrence rule’s calendar.

var recurrenceEnd: EKRecurrenceEnd?

Indicates when the recurrence rule ends.

var frequency: EKRecurrenceFrequency

The frequency of the recurrence rule.

var interval: Int

Specifies how often the recurrence rule repeats over the unit of time indicated by its frequency.

var firstDayOfTheWeek: Int

Indicates which day of the week the recurrence rule treats as the first day of the week.

var daysOfTheWeek: [EKRecurrenceDayOfWeek]?

The days of the week associated with the recurrence rule, as an array of EKRecurrenceDayOfWeek objects.

var daysOfTheMonth: [NSNumber]?

The days of the month associated with the recurrence rule, as an array of `NSNumber` objects.

var daysOfTheYear: [NSNumber]?

The days of the year associated with the recurrence rule, as an array of `NSNumber` objects.

var weeksOfTheYear: [NSNumber]?

The weeks of the year associated with the recurrence rule, as an array of `NSNumber` objects.

var monthsOfTheYear: [NSNumber]?

The months of the year associated with the recurrence rule, as an array of `NSNumber` objects.

var setPositions: [NSNumber]?

An array of ordinal numbers that filters which recurrences to include in the recurrence rule’s frequency.

func EK_LOSE_FRACTIONAL_SECONDS_DO_NOT_USE()

A deprecated function.

Deprecated

## Relationships

### Inherits From

- EKObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Recurrence

Creating a recurring event

Set up an event or reminder that repeats.

class EKRecurrenceDayOfWeek

A class that represents the day of the week.

class EKRecurrenceEnd

A class that defines the end of a recurrence rule.

