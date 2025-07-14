

- Foundation
- NSCalendar
-  getEra(\_:yearForWeekOfYear:weekOfYear:weekday:from:) 

Instance Method

# getEra(\_:yearForWeekOfYear:weekOfYear:weekday:from:)

Returns by reference the era, year, week of year, and weekday component values for a given date.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func getEra(
    _ eraValuePointer: UnsafeMutablePointer?,
    yearForWeekOfYear yearValuePointer: UnsafeMutablePointer?,
    weekOfYear weekValuePointer: UnsafeMutablePointer?,
    weekday weekdayValuePointer: UnsafeMutablePointer?,
    from date: Date
)
```

## Parameters 

`eraValuePointer`  

Upon return, contains the era of the given date.

`yearValuePointer`  

Upon return, contains the year of the given date.

`weekValuePointer`  

Upon return, contains the week of the given date.

`weekdayValuePointer`  

Upon return, contains the weekday of the given date.

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

func getHour(UnsafeMutablePointer&lt;Int>?, minute: UnsafeMutablePointer&lt;Int>?, second: UnsafeMutablePointer&lt;Int>?, nanosecond: UnsafeMutablePointer&lt;Int>?, from: Date)

Returns by reference the hour, minute, second, and nanosecond component values for a given date.

