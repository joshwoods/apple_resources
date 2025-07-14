

- EventKit
- EKRecurrenceRule
-  daysOfTheMonth 

Instance Property

# daysOfTheMonth

The days of the month associated with the recurrence rule, as an array of `NSNumber` objects.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.8+visionOS 1.0+watchOS 2.0+

``` source
var daysOfTheMonth: [NSNumber]? { get }
```

## Discussion

Values can be from `1` to `31` and from `-1` to `-31`. This property value is valid only for recurrence rules that were initialized with specific days of the month and a frequency type of EKRecurrenceFrequency.monthly.

Negative values indicate counting backwards from the end of the month.

## See Also

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

