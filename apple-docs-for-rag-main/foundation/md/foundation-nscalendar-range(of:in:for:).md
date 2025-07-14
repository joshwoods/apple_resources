

- Foundation
- NSCalendar
-  range(of:in:for:) 

Instance Method

# range(of:in:for:)

Returns the range of absolute time values that a smaller calendar unit (such as a day) can take on in a larger calendar unit (such as a month) that includes a specified absolute time.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func range(
    of smaller: NSCalendar.Unit,
    in larger: NSCalendar.Unit,
    for date: Date
) -> NSRange
```

## Parameters 

`smaller`  

The smaller calendar unit.

`larger`  

The larger calendar unit.

`date`  

The absolute time for which the calculation is performed.

## Return Value

The range of absolute time values `smaller` can take on in `larger` at the time specified by `date`. Returns `{NSNotFound, NSNotFound`} if `larger` is not logically bigger than `smaller` in the calendar, or the given combination of units does not make sense (or is a computation which is undefined).

## Discussion

You can use this method to calculate, for example, the range the Day unit can take on in the Month in which `date` lies.

## See Also

### Getting Calendar Information

var calendarIdentifier: NSCalendar.Identifier

An identifier for the calendar.

var firstWeekday: Int

The index of the first weekday of the receiver.

var locale: Locale?

The locale of the receiver.

var timeZone: TimeZone

The time zone for the calendar.

func maximumRange(of: NSCalendar.Unit) -> NSRange

Returns the maximum range limits of the values that a given unit can take on.

func minimumRange(of: NSCalendar.Unit) -> NSRange

Returns the minimum range limits of the values that a given unit can take on.

var minimumDaysInFirstWeek: Int

The minimum number of days in the first week of the receiver.

func ordinality(of: NSCalendar.Unit, in: NSCalendar.Unit, for: Date) -> Int

Returns, for a given absolute time, the ordinal number of a smaller calendar unit (such as a day) within a specified larger calendar unit (such as a week).

func range(of: NSCalendar.Unit, start: AutoreleasingUnsafeMutablePointer&lt;NSDate?>?, interval: UnsafeMutablePointer&lt;TimeInterval>?, for: Date) -> Bool

Returns by reference the starting time and duration of a given calendar unit that contains a given date.

func range(ofWeekendStart: AutoreleasingUnsafeMutablePointer&lt;NSDate?>?, interval: UnsafeMutablePointer&lt;TimeInterval>?, containing: Date) -> Bool

Returns whether a given date falls within a weekend period, and if so, returns by reference the start date and time interval of the weekend range.

struct Unit

Calendrical units such as year, month, day and hour.

