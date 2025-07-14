

- Foundation
- NSCalendar
- NSCalendar.Unit
-  weekday 

Type Property

# weekday

Identifier for the weekday unit.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static var weekday: NSCalendar.Unit { get }
```

## Discussion

The corresponding value is an `NSInteger`. Equal to `kCFCalendarUnitWeekday`. The weekday units are the numbers `1` through `N` (where for the Gregorian calendar `N`=`7` and `1` is Sunday).

## See Also

### Specifying Weeks and Days

static var weekOfYear: NSCalendar.Unit

Identifier for the week of the year calendar unit.

static var weekOfMonth: NSCalendar.Unit

Identifier for the week of the month calendar unit.

static var weekdayOrdinal: NSCalendar.Unit

Identifier for the ordinal weekday unit.

static var day: NSCalendar.Unit

Identifier for the day unit.

static var weekOfYear: NSCalendar.Unit

Identifier for the week of the year calendar unit.

static var weekOfMonth: NSCalendar.Unit

Identifier for the week of the month calendar unit.

static var weekdayOrdinal: NSCalendar.Unit

Identifier for the ordinal weekday unit.

static var day: NSCalendar.Unit

Identifier for the day unit.

