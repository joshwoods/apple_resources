

- Foundation
- NSCalendar
-  date(era:yearForWeekOfYear:weekOfYear:weekday:hour:minute:second:nanosecond:) 

Instance Method

# date(era:yearForWeekOfYear:weekOfYear:weekday:hour:minute:second:nanosecond:)

Returns a new date created with the given components base on a week-of-year value.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func date(
    era eraValue: Int,
    yearForWeekOfYear yearValue: Int,
    weekOfYear weekValue: Int,
    weekday weekdayValue: Int,
    hour hourValue: Int,
    minute minuteValue: Int,
    second secondValue: Int,
    nanosecond nanosecondValue: Int
) -> Date?
```

## Parameters 

`eraValue`  

The value for the era component.

`yearValue`  

The value for the year component.

`weekValue`  

The value for the week-of-year component.

`weekdayValue`  

The value to use as the weekday.

`hourValue`  

The value for the hour component.

`minuteValue`  

The value for the minute component.

`secondValue`  

The value for the second component.

`nanosecondValue`  

The value for the nanosecond component.

## Return Value

A new `NSDate` instance created with the given components based on a week-of-year calculation, or `nil` if the components do not correspond to a valid date.

## See Also

### Calculating Dates

func date(from: DateComponents) -> Date?

Returns a date representing the absolute time calculated from given components.

func date(byAdding: DateComponents, to: Date, options: NSCalendar.Options) -> Date?

Returns a date representing the absolute time calculated by adding given components to a given date.

func date(byAdding: NSCalendar.Unit, value: Int, to: Date, options: NSCalendar.Options) -> Date?

Returns a date representing the absolute time calculated by adding the value of a given component to a given date.

func date(bySettingHour: Int, minute: Int, second: Int, of: Date, options: NSCalendar.Options) -> Date?

Creates a new date calculated with the given time.

func date(bySettingUnit: NSCalendar.Unit, value: Int, of: Date, options: NSCalendar.Options) -> Date?

Returns a new date representing the date calculated by setting a specific component of a given date to a given value, while trying to keep lower components the same.

func date(era: Int, year: Int, month: Int, day: Int, hour: Int, minute: Int, second: Int, nanosecond: Int) -> Date?

Returns a date created with the given components.

func nextWeekendStart(AutoreleasingUnsafeMutablePointer&lt;NSDate?>?, interval: UnsafeMutablePointer&lt;TimeInterval>?, options: NSCalendar.Options, after: Date) -> Bool

Returns by reference the starting date and time interval range of the next weekend period after a given date.

