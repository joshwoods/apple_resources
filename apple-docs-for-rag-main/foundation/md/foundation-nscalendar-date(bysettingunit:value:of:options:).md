

- Foundation
- NSCalendar
-  date(bySettingUnit:value:of:options:) 

Instance Method

# date(bySettingUnit:value:of:options:)

Returns a new date representing the date calculated by setting a specific component of a given date to a given value, while trying to keep lower components the same.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func date(
    bySettingUnit unit: NSCalendar.Unit,
    value v: Int,
    of date: Date,
    options opts: NSCalendar.Options = []
) -> Date?
```

## Parameters 

`unit`  

The unit to set with the given value. For possible values, see NSCalendar.Unit.

`v`  

The value to set for the given calendar unit.

`date`  

The date to use to perform the calculation.

`opts`  

Options for the calculation. For possible values, see NSCalendar.Options.

## Return Value

A new `NSDate` instance representing the date calculated by setting a specific component of a given date to a given value. If the unit already has that value, this may result in a date which is the same as the given date. If no such time exists for the specified components, the next available date is returned, which may be on a different calendar day.

## Discussion

Changing a component’s value often requires higher or coupled components to change as well. For example, setting the `weekday` to “Thursday” will require the `day` component to change its value, and possibly the `month` and `year` as well. You can use the nextDate(after:matching:value:options:) method to specify more precise behavior for determining the next or previous date for a given date component.

## See Also

### Related Documentation

func nextDate(after: Date, matching: NSCalendar.Unit, value: Int, options: NSCalendar.Options) -> Date?

Returns the next date after a given date matching the given calendar unit value.

### Calculating Dates

func date(from: DateComponents) -> Date?

Returns a date representing the absolute time calculated from given components.

func date(byAdding: DateComponents, to: Date, options: NSCalendar.Options) -> Date?

Returns a date representing the absolute time calculated by adding given components to a given date.

func date(byAdding: NSCalendar.Unit, value: Int, to: Date, options: NSCalendar.Options) -> Date?

Returns a date representing the absolute time calculated by adding the value of a given component to a given date.

func date(bySettingHour: Int, minute: Int, second: Int, of: Date, options: NSCalendar.Options) -> Date?

Creates a new date calculated with the given time.

func date(era: Int, year: Int, month: Int, day: Int, hour: Int, minute: Int, second: Int, nanosecond: Int) -> Date?

Returns a date created with the given components.

func date(era: Int, yearForWeekOfYear: Int, weekOfYear: Int, weekday: Int, hour: Int, minute: Int, second: Int, nanosecond: Int) -> Date?

Returns a new date created with the given components base on a week-of-year value.

func nextWeekendStart(AutoreleasingUnsafeMutablePointer&lt;NSDate?>?, interval: UnsafeMutablePointer&lt;TimeInterval>?, options: NSCalendar.Options, after: Date) -> Bool

Returns by reference the starting date and time interval range of the next weekend period after a given date.

