

- Foundation
- Dates and Times
- NSCalendar
-  NSWrapCalendarComponents 

API Collection

# NSWrapCalendarComponents

A legacy constant used to control overflow in date calculations.

## Overview

Deprecated

Use wrapComponents instead.

## Topics

### Constants

var NSWrapCalendarComponents: Int

Specifies that the components specified for an `NSDateComponents` object should be incremented and wrap around to zero/one on overflow, but should not cause higher units to be incremented.

Deprecated

## See Also

### Scanning Dates

func startOfDay(for: Date) -> Date

Returns the first moment of a given date as a date instance.

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

