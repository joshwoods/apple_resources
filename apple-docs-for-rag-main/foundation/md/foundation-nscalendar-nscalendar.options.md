

- Foundation
- NSCalendar
-  NSCalendar.Options 

Structure

# NSCalendar.Options

The options for arithmetic operations involving calendars.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
struct Options
```

## Topics

### Initializers

init(rawValue: UInt)

### Constants

static var wrapComponents: NSCalendar.Options

Specifies that the components specified for an `NSDateComponents` object should be incremented and wrap around to zero/one on overflow, but should not cause higher units to be incremented.

static var matchStrictly: NSCalendar.Options

Specifies that the operation should travel as far forward or backward as necessary looking for a match.

static var searchBackwards: NSCalendar.Options

Specifies that the operation should travel backwards to find the previous match before the given date.

static var matchPreviousTimePreservingSmallerUnits: NSCalendar.Options

Specifies that, when there is no matching time before the end of the next instance of the next highest unit specified in the given `NSDateComponents` object, this method uses the *previous* existing value of the missing unit and preserves the lower units’ values.

static var matchNextTimePreservingSmallerUnits: NSCalendar.Options

Specifies that, when there is no matching time before the end of the next instance of the next highest unit specified in the given `NSDateComponents` object, this method uses the *next* existing value of the missing unit and preserves the lower units’ values.

static var matchNextTime: NSCalendar.Options

Specifies that, when there is no matching time before the end of the next instance of the next highest unit specified in the given `NSDateComponents` object, this method uses the *next* existing value of the missing unit and *does not* preserve the lower units’ values.

static var matchFirst: NSCalendar.Options

Specifies that, if there are two or more matching times, the operation should return the first occurrence.

static var matchLast: NSCalendar.Options

Specifies that, if there are two or more matching times, the operation should return the last occurrence.

static var wrapComponents: NSCalendar.Options

Specifies that the components specified for an `NSDateComponents` object should be incremented and wrap around to zero/one on overflow, but should not cause higher units to be incremented.

static var matchStrictly: NSCalendar.Options

Specifies that the operation should travel as far forward or backward as necessary looking for a match.

static var searchBackwards: NSCalendar.Options

Specifies that the operation should travel backwards to find the previous match before the given date.

static var matchPreviousTimePreservingSmallerUnits: NSCalendar.Options

Specifies that, when there is no matching time before the end of the next instance of the next highest unit specified in the given `NSDateComponents` object, this method uses the *previous* existing value of the missing unit and preserves the lower units’ values.

static var matchNextTimePreservingSmallerUnits: NSCalendar.Options

Specifies that, when there is no matching time before the end of the next instance of the next highest unit specified in the given `NSDateComponents` object, this method uses the *next* existing value of the missing unit and preserves the lower units’ values.

static var matchNextTime: NSCalendar.Options

Specifies that, when there is no matching time before the end of the next instance of the next highest unit specified in the given `NSDateComponents` object, this method uses the *next* existing value of the missing unit and *does not* preserve the lower units’ values.

static var matchFirst: NSCalendar.Options

Specifies that, if there are two or more matching times, the operation should return the first occurrence.

static var matchLast: NSCalendar.Options

Specifies that, if there are two or more matching times, the operation should return the last occurrence.

var NSWrapCalendarComponents: Int

Specifies that the components specified for an `NSDateComponents` object should be incremented and wrap around to zero/one on overflow, but should not cause higher units to be incremented.

Deprecated

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

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

NSWrapCalendarComponents

A legacy constant used to control overflow in date calculations.

