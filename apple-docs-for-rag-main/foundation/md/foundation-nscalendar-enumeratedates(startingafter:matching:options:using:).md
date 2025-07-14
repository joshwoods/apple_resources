

- Foundation
- NSCalendar
-  enumerateDates(startingAfter:matching:options:using:) 

Instance Method

# enumerateDates(startingAfter:matching:options:using:)

Computes the dates that match (or most closely match) a given set of components, and calls the block once for each of them, until the enumeration is stopped.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func enumerateDates(
    startingAfter start: Date,
    matching comps: DateComponents,
    options opts: NSCalendar.Options = [],
    using block: (Date?, Bool, UnsafeMutablePointer) -> Void
)
```

## Parameters 

`start`  

The date for which to perform the calculation.

`comps`  

The date components to match. If no components are specified, the enumeration will not be executed. If the `nanoseconds` component is set to a nonzero value, the resulting dates will have floating point `seconds` values that most closely match the specified `nanoseconds` value. Otherwise, the resulting dates will have an integer `seconds` value.

`opts`  

Options for the enumeration. For possible values, see NSCalendar.Options. For usage, see *Discussion* below.

`block`  

The block to apply to each enumerated date. The block takes three arguments:

date  
The enumerated date.

idx  
Whether `date` exactly matches the specified date components.

stop  
A reference to a Boolean value. The block can set the value to true to stop further processing of the array. The stop argument is an out-only argument. You should only ever set this Boolean to true within the Block.

## Discussion

Executes a given block with dates that most closely match a given set of components after a given date, until the enumeration is stopped.

Strict & Non-Strict Matching

If you specify a strict matching option (matchStrictly), this method searches as far as necessary looking for a match, up to a an implementation-defined limit. If an exact match is not possible, `nil` is passed to the `date` argument of the block, and the enumeration is stopped. Otherwise, this method searches as far as the next instance of the next highest calendar unit in the given `NSDateComponents` object.

If you do not specify a strict matching option, you must specify one of the following options, or else an illegal argument exception will be thrown:

matchPreviousTimePreservingSmallerUnits  
If specified, and there is no matching time before the end of the next instance of the next highest unit specified in the given `NSDateComponents` object, this method uses the *previous* existing value of the missing unit and preserves the lower units’ values.

matchNextTimePreservingSmallerUnits  
If specified, and there is no matching time before the end of the next instance of the next highest unit specified in the given `NSDateComponents` object, this method uses the *next* existing value of the missing unit and preserves the lower units’ values.

matchNextTime  
If specified, and there is no matching time before the end of the next instance of the next highest unit specified in the given `NSDateComponents` object, this method uses the *next* existing value of the missing unit and *does not* preserve the lower units’ values.

For example, if the date “February 29th” does not exist for a particular year, a non-strict match would return “February 28th” of that year instead.

As another example, if the time “2:37AM” does not exist for a particular day, such as when advancing by an hour at the beginning of Daylight Savings Time, the following is true:

- If strict matching is specified, “2:37AM” on the following the next day is used.

- If matchPreviousTimePreservingSmallerUnits is specified, “1:37AM” would be used instead, if that time exists.

- If matchNextTimePreservingSmallerUnits is specified, the date at the time “3:37AM” would be used instead, if that time exists.

- If matchNextTime is specified, the date at the time “3:00AM” would be used instead, if that time exists.

Matching First or Last Occurrence

If you specify a “match first” option (matchFirst) and there are two or more matching times (that is, all components are the same) before the end of the next instance of the next highest unit specified in the given `NSDateComponents` object, this method uses the *first* occurrence.

If you specify a “match last” option (matchLast) and there are two or more matching times (that is, all components are the same) before the end of the next instance of the next highest unit specified in the given `NSDateComponents` object, this method uses the *last* occurrence.

If neither “match first” or “match last” options are specified or both options are specified, this method behaves as if matchFirst was specified.

There is no option to return middle occurrences of more than two occurrences of a matching time, if such exist.

For example, when Daylight Savings Time ends, clocks are set back by one hour at 2:00AM, such that times between 1:00AM and 1:59AM occur twice that day. The matchFirst and matchLast search options return the first and last occurrence of these times.

Forward & Backward Search

If you specify a backward search option (searchBackwards), this method will search for previous matches before the given date. This method will return the same results as if the search were made in the forward direction from the distant past, but with the results in reverse order starting with the match most recent to the given date. That is, when searching backwards for a particular hour with no specified minute or second value, the resulting time is not “59” minutes and “59” seconds for the matching hour. When enumerating dates that repeat a time, such as when the clock turns back to 1:00AM from 2:00AM when Daylight Savings Time ends, the “first” time is determined as if the search were performed in the forwards direction.

For example, given a date with a time of “5:00AM” when searching for a minute component equal to 30, a forward search returns the time “5:30AM” and a backward search returns “4:30AM”.

## See Also

### Scanning Dates

func startOfDay(for: Date) -> Date

Returns the first moment of a given date as a date instance.

func nextDate(after: Date, matching: DateComponents, options: NSCalendar.Options) -> Date?

Returns the next date after a given date matching the given components.

func nextDate(after: Date, matchingHour: Int, minute: Int, second: Int, options: NSCalendar.Options) -> Date?

Returns the next date after a given date that matches the given hour, minute, and second, component values.

func nextDate(after: Date, matching: NSCalendar.Unit, value: Int, options: NSCalendar.Options) -> Date?

Returns the next date after a given date matching the given calendar unit value.

struct Options

The options for arithmetic operations involving calendars.

NSWrapCalendarComponents

A legacy constant used to control overflow in date calculations.

