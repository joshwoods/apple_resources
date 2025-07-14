

- Foundation
- NSCalendar
-  minimumDaysInFirstWeek 

Instance Property

# minimumDaysInFirstWeek

The minimum number of days in the first week of the receiver.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var minimumDaysInFirstWeek: Int { get set }
```

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

func ordinality(of: NSCalendar.Unit, in: NSCalendar.Unit, for: Date) -> Int

Returns, for a given absolute time, the ordinal number of a smaller calendar unit (such as a day) within a specified larger calendar unit (such as a week).

func range(of: NSCalendar.Unit, in: NSCalendar.Unit, for: Date) -> NSRange

Returns the range of absolute time values that a smaller calendar unit (such as a day) can take on in a larger calendar unit (such as a month) that includes a specified absolute time.

func range(of: NSCalendar.Unit, start: AutoreleasingUnsafeMutablePointer&lt;NSDate?>?, interval: UnsafeMutablePointer&lt;TimeInterval>?, for: Date) -> Bool

Returns by reference the starting time and duration of a given calendar unit that contains a given date.

func range(ofWeekendStart: AutoreleasingUnsafeMutablePointer&lt;NSDate?>?, interval: UnsafeMutablePointer&lt;TimeInterval>?, containing: Date) -> Bool

Returns whether a given date falls within a weekend period, and if so, returns by reference the start date and time interval of the weekend range.

struct Unit

Calendrical units such as year, month, day and hour.

