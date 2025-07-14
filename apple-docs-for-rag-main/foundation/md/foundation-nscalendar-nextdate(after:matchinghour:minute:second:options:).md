

- Foundation
- NSCalendar
-  nextDate(after:matchingHour:minute:second:options:) 

Instance Method

# nextDate(after:matchingHour:minute:second:options:)

Returns the next date after a given date that matches the given hour, minute, and second, component values.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func nextDate(
    after date: Date,
    matchingHour hourValue: Int,
    minute minuteValue: Int,
    second secondValue: Int,
    options: NSCalendar.Options = []
) -> Date?
```

## Parameters 

`date`  

The date for which to perform the calculation.

`hourValue`  

The value for the hour component.

`minuteValue`  

The value for the minute component.

`secondValue`  

The value for the second component.

`options`  

Options for the calculation. For possible values, see NSCalendar.Options.

## Return Value

A new `NSDate` object.

## See Also

### Scanning Dates

func startOfDay(for: Date) -> Date

Returns the first moment of a given date as a date instance.

func enumerateDates(startingAfter: Date, matching: DateComponents, options: NSCalendar.Options, using: (Date?, Bool, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Computes the dates that match (or most closely match) a given set of components, and calls the block once for each of them, until the enumeration is stopped.

func nextDate(after: Date, matching: DateComponents, options: NSCalendar.Options) -> Date?

Returns the next date after a given date matching the given components.

func nextDate(after: Date, matching: NSCalendar.Unit, value: Int, options: NSCalendar.Options) -> Date?

Returns the next date after a given date matching the given calendar unit value.

struct Options

The options for arithmetic operations involving calendars.

NSWrapCalendarComponents

A legacy constant used to control overflow in date calculations.

