

- EventKit
-  EKRecurrenceFrequency 

Enumeration

# EKRecurrenceFrequency

The frequency for recurrence rules.

iOSiPadOSMac CatalystmacOSvisionOSwatchOS

``` source
enum EKRecurrenceFrequency
```

## Mentioned in 

Creating a recurring event

## Topics

### Constants

case daily

Indicates a daily recurrence rule.

case weekly

Indicates a weekly recurrence rule.

case monthly

Indicates a monthly recurrence rule.

case yearly

Indicates a yearly recurrence rule.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Accessing Recurrence Rule Properties

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

