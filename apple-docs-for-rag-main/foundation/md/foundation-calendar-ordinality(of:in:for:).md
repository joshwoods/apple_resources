

- Foundation
- Calendar
-  ordinality(of:in:for:) 

Instance Method

# ordinality(of:in:for:)

Returns, for a given absolute time, the ordinal number of a smaller calendar component (such as a day) within a specified larger calendar component (such as a week).

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func ordinality(
    of smaller: Calendar.Component,
    in larger: Calendar.Component,
    for date: Date
) -> Int?
```

## Parameters 

`smaller`  

The smaller calendar component.

`larger`  

The larger calendar component.

`date`  

The absolute time for which the calculation is performed.

## Return Value

The ordinal number of smaller within larger at the time specified by date. Returns `nil` if larger is not logically bigger than smaller in the calendar, or the given combination of components does not make sense (or is a computation which is undefined).

## Discussion

The ordinality is in most cases not the same as the decomposed value of the component. Typically return values are 1 and greater. For example, the time 00:45 is in the first hour of the day, and for components `hour` and `day` respectively, the result would be 1. An exception is the week-in-month calculation, which returns 0 for days before the first week in the month containing the date.

Note

Some computations can take a relatively long time.

## See Also

### Getting Calendar Information

var identifier: Calendar.Identifier

The identifier of the calendar.

var locale: Locale?

The locale of the calendar.

var firstWeekday: Int

The first day of the week for the calendar.

var minimumDaysInFirstWeek: Int

The number of minimum days in the first week.

var timeZone: TimeZone

The time zone of the calendar.

func maximumRange(of: Calendar.Component) -> Range&lt;Int>?

The maximum range limits of the values that a given component can take on.

func minimumRange(of: Calendar.Component) -> Range&lt;Int>?

Returns the minimum range limits of the values that a given component can take on.

func range(of: Calendar.Component, in: Calendar.Component, for: Date) -> Range&lt;Int>?

Returns the range of absolute time values that a smaller calendar component (such as a day) can take on in a larger calendar component (such as a month) that includes a specified absolute time.

