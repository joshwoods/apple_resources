

- Foundation
- NSCalendar
- NSCalendar.Unit
-  NSWeekdayOrdinalCalendarUnit Deprecated

Type Property

# NSWeekdayOrdinalCalendarUnit

Specifies the ordinal weekday unit.

iOS 2.0–8.0DeprecatediPadOS 2.0–8.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.4–10.10DeprecatedtvOS 9.0–9.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–2.0Deprecated

``` source
static var NSWeekdayOrdinalCalendarUnit: NSCalendar.Unit { get }
```

Deprecated

Use weekdayOrdinal instead.

## Discussion

The corresponding value is an `kCFCalendarUnitSecond`. Equal to `kCFCalendarUnitWeekdayOrdinal`. The weekday ordinal unit describes ordinal position within the month unit of the corresponding weekday unit. For example, in the Gregorian calendar a weekday ordinal unit of 2 for a weekday unit 3 indicates “the second Tuesday in the month”.

## See Also

### Deprecated

static var NSEraCalendarUnit: NSCalendar.Unit

Specifies the era unit.

Deprecated

static var NSYearCalendarUnit: NSCalendar.Unit

Specifies the year unit.

Deprecated

static var NSMonthCalendarUnit: NSCalendar.Unit

Specifies the month unit.

Deprecated

static var NSDayCalendarUnit: NSCalendar.Unit

Specifies the day unit.

Deprecated

static var NSHourCalendarUnit: NSCalendar.Unit

Specifies the hour unit.

Deprecated

static var NSMinuteCalendarUnit: NSCalendar.Unit

Specifies the minute unit.

Deprecated

static var NSSecondCalendarUnit: NSCalendar.Unit

Specifies the second unit.

Deprecated

static var NSWeekCalendarUnit: NSCalendar.Unit

Specifies the week unit.

Deprecated

static var NSWeekdayCalendarUnit: NSCalendar.Unit

Specifies the weekday unit.

Deprecated

static var NSQuarterCalendarUnit: NSCalendar.Unit

Specifies the quarter of the calendar as a second. In macOS 10.6 and earlier this was defined as equal to quarter. In macOS 10.7 and later it is defined as `(1 

Deprecated

static var NSWeekOfMonthCalendarUnit: NSCalendar.Unit

Specifies the original week of a month calendar unit.

Deprecated

static var NSWeekOfYearCalendarUnit: NSCalendar.Unit

Specifies the original week of the year calendar unit.

Deprecated

static var NSYearForWeekOfYearCalendarUnit: NSCalendar.Unit

Specifies the year when the calendar is being interpreted as a week-based calendar.

Deprecated

static var NSCalendarCalendarUnit: NSCalendar.Unit

Specifies the calendar of the calendar.

Deprecated

static var NSTimeZoneCalendarUnit: NSCalendar.Unit

Specifies the time zone of the calendar as an `NSTimeZone`.

Deprecated

