

- Foundation
- NSCalendar
-  date(\_:matchesComponents:) 

Instance Method

# date(\_:matchesComponents:)

Returns whether a given date matches all of the given date components.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func date(
    _ date: Date,
    matchesComponents components: DateComponents
) -> Bool
```

## Parameters 

`date`  

The date for which to perform the calculation.

`components`  

The date components to match.

## Return Value

true if the given date matches the given components, otherwise false.

## Discussion

This method is useful for determining whether dates calculated by methods like nextDate(after:matching:value:options:) or enumerateDates(startingAfter:matching:options:using:) are exact, or required an adjustment due to a nonexistent time.

## See Also

### Related Documentation

func nextDate(after: Date, matching: NSCalendar.Unit, value: Int, options: NSCalendar.Options) -> Date?

Returns the next date after a given date matching the given calendar unit value.

func enumerateDates(startingAfter: Date, matching: DateComponents, options: NSCalendar.Options, using: (Date?, Bool, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Computes the dates that match (or most closely match) a given set of components, and calls the block once for each of them, until the enumeration is stopped.

### Extracting Components

func component(NSCalendar.Unit, from: Date) -> Int

Returns the specified date component from a given date.

func components(NSCalendar.Unit, from: Date) -> DateComponents

Returns the date components representing a given date.

func components(NSCalendar.Unit, from: Date, to: Date, options: NSCalendar.Options) -> DateComponents

Returns the difference between two supplied dates as date components.

func components(NSCalendar.Unit, from: DateComponents, to: DateComponents, options: NSCalendar.Options) -> DateComponents

Returns the difference between start and end dates given as date components.

func components(in: TimeZone, from: Date) -> DateComponents

Returns all the date components of a date, as if in a given time zone (instead of the receiving calendar’s time zone).

func getEra(UnsafeMutablePointer&lt;Int>?, year: UnsafeMutablePointer&lt;Int>?, month: UnsafeMutablePointer&lt;Int>?, day: UnsafeMutablePointer&lt;Int>?, from: Date)

Returns by reference the era, year, week of year, and weekday component values for a given date.

func getEra(UnsafeMutablePointer&lt;Int>?, yearForWeekOfYear: UnsafeMutablePointer&lt;Int>?, weekOfYear: UnsafeMutablePointer&lt;Int>?, weekday: UnsafeMutablePointer&lt;Int>?, from: Date)

Returns by reference the era, year, week of year, and weekday component values for a given date.

func getHour(UnsafeMutablePointer&lt;Int>?, minute: UnsafeMutablePointer&lt;Int>?, second: UnsafeMutablePointer&lt;Int>?, nanosecond: UnsafeMutablePointer&lt;Int>?, from: Date)

Returns by reference the hour, minute, second, and nanosecond component values for a given date.

