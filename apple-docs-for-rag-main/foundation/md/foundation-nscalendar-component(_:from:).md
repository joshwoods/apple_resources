

- Foundation
- NSCalendar
-  component(\_:from:) 

Instance Method

# component(\_:from:)

Returns the specified date component from a given date.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func component(
    _ unit: NSCalendar.Unit,
    from date: Date
) -> Int
```

## Parameters 

`unit`  

The component to return. For possible values, see NSCalendar.Unit.

`date`  

The date for which to perform the calculation.

## Return Value

An `NSInteger` value for the requested component.

## See Also

### Extracting Components

func date(Date, matchesComponents: DateComponents) -> Bool

Returns whether a given date matches all of the given date components.

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

