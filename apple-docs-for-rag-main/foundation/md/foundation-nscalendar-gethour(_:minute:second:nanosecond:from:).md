

- Foundation
- NSCalendar
-  getHour(\_:minute:second:nanosecond:from:) 

Instance Method

# getHour(\_:minute:second:nanosecond:from:)

Returns by reference the hour, minute, second, and nanosecond component values for a given date.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func getHour(
    _ hourValuePointer: UnsafeMutablePointer?,
    minute minuteValuePointer: UnsafeMutablePointer?,
    second secondValuePointer: UnsafeMutablePointer?,
    nanosecond nanosecondValuePointer: UnsafeMutablePointer?,
    from date: Date
)
```

## Parameters 

`hourValuePointer`  

Upon return, contains the hour of the given date.

`minuteValuePointer`  

Upon return, contains the minute of the given date.

`secondValuePointer`  

Upon return, contains the second of the given date.

`nanosecondValuePointer`  

Upon return, contains the nanosecond of the given date.

`date`  

The date for which to perform the calculation.

## Discussion

Pass `NULL` to ignore any individual component parameter.

This is a convenience method for getting the time components of a given date using components(_:from:)

## See Also

### Extracting Components

func date(Date, matchesComponents: DateComponents) -> Bool

Returns whether a given date matches all of the given date components.

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

