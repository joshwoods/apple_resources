

- Foundation
- NSCalendar
-  components(\_:from:to:options:) 

Instance Method

# components(\_:from:to:options:)

Returns the difference between start and end dates given as date components.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func components(
    _ unitFlags: NSCalendar.Unit,
    from startingDateComp: DateComponents,
    to resultDateComp: DateComponents,
    options: NSCalendar.Options = []
) -> DateComponents
```

## Parameters 

`unitFlags`  

Specifies the components for the returned `NSDateComponents` object.

`startingDateComp`  

The start date for the calculation as an `NSDateComponents` object.

`resultDateComp`  

The end date for the calculation as an `NSDateComponents` object.

`options`  

The `options` parameter is currently unused.

## Return Value

An `NSDateComponents` object whose components are specified by `unitFlags` and calculated from the difference between the `startingDateComp` and `resultDateComp` using the options specified by `options`. Returns `nil` if either date falls outside the defined range of the receiver or if the computation cannot be performed.

## Discussion

If an `NSDateComponents` object does not specify a value for a calendar unit required to determine an absolute date, the base value of that unit is assumed. For example, given an `NSDateComponents` object with only a `year` and a `month` specified, the resulting `NSDate` object would be constructed using a `day` value of `1` and `hour`, `minute`, `second` and `nanosecond` values of `0`. Passing an `NSDateComponents` argument with an unspecified `era` or `year` value is not advised.

If an `NSDateComponents` object’s `timeZone` property is set, the time zone property value will be used in the calculation. If an `NSDateComponents` object’s `calendar` property is set, the calendar property value will be used instead of the receiving calendar. If both an `NSDateComponents` object’s `timeZone` and `calendar` properties are set, the time zone property value overrides the time zone of the calendar property value.

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

func components(in: TimeZone, from: Date) -> DateComponents

Returns all the date components of a date, as if in a given time zone (instead of the receiving calendar’s time zone).

func getEra(UnsafeMutablePointer&lt;Int>?, year: UnsafeMutablePointer&lt;Int>?, month: UnsafeMutablePointer&lt;Int>?, day: UnsafeMutablePointer&lt;Int>?, from: Date)

Returns by reference the era, year, week of year, and weekday component values for a given date.

func getEra(UnsafeMutablePointer&lt;Int>?, yearForWeekOfYear: UnsafeMutablePointer&lt;Int>?, weekOfYear: UnsafeMutablePointer&lt;Int>?, weekday: UnsafeMutablePointer&lt;Int>?, from: Date)

Returns by reference the era, year, week of year, and weekday component values for a given date.

func getHour(UnsafeMutablePointer&lt;Int>?, minute: UnsafeMutablePointer&lt;Int>?, second: UnsafeMutablePointer&lt;Int>?, nanosecond: UnsafeMutablePointer&lt;Int>?, from: Date)

Returns by reference the hour, minute, second, and nanosecond component values for a given date.

