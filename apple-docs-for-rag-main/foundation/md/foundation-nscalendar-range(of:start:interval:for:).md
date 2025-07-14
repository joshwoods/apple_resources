

- Foundation
- NSCalendar
-  range(of:start:interval:for:) 

Instance Method

# range(of:start:interval:for:)

Returns by reference the starting time and duration of a given calendar unit that contains a given date.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func range(
    of unit: NSCalendar.Unit,
    start datep: AutoreleasingUnsafeMutablePointer?,
    interval tip: UnsafeMutablePointer?,
    for date: Date
) -> Bool
```

## Parameters 

`unit`  

A calendar unit (see NSCalendar.Unit for possible values).

`datep`  

Upon return, contains the starting time of the calendar unit `unit` that contains the date `date`

`tip`  

Upon return, contains the duration of the calendar unit `unit` that contains the date `date`

`date`  

A date.

## Return Value

true if the starting time and duration of a unit could be calculated, otherwise false.

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

func range(of: NSCalendar.Unit, in: NSCalendar.Unit, for: Date) -> NSRange

Returns the range of absolute time values that a smaller calendar unit (such as a day) can take on in a larger calendar unit (such as a month) that includes a specified absolute time.

func range(ofWeekendStart: AutoreleasingUnsafeMutablePointer&lt;NSDate?>?, interval: UnsafeMutablePointer&lt;TimeInterval>?, containing: Date) -> Bool

Returns whether a given date falls within a weekend period, and if so, returns by reference the start date and time interval of the weekend range.

struct Unit

Calendrical units such as year, month, day and hour.

