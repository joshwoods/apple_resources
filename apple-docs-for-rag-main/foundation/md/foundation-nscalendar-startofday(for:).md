

- Foundation
- NSCalendar
-  startOfDay(for:) 

Instance Method

# startOfDay(for:)

Returns the first moment of a given date as a date instance.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func startOfDay(for date: Date) -> Date
```

## Parameters 

`date`  

The date for which to perform the calculation.

## Return Value

An `NSDate` instance representing the first moment date of the given date.

## Discussion

For example, passing `[NSDate date]` for the `date` parameter would give you the start of “today.”

### Special Considerations

If there were two midnights, this method returns the first. If there was none, it returns the first moment that did exist.

## See Also

### Scanning Dates

func enumerateDates(startingAfter: Date, matching: DateComponents, options: NSCalendar.Options, using: (Date?, Bool, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Computes the dates that match (or most closely match) a given set of components, and calls the block once for each of them, until the enumeration is stopped.

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

