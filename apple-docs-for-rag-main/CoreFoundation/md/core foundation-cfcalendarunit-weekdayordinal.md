

- Core Foundation
- CFCalendarUnit
-  weekdayOrdinal 

Type Property

# weekdayOrdinal

Specifies the ordinal weekday unit.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
static var weekdayOrdinal: CFCalendarUnit { get }
```

## Discussion

The weekday ordinal unit describes ordinal position within the month unit of the corresponding weekday unit. For example, in the Gregorian calendar a weekday ordinal unit of `2` for a weekday unit `3` indicates “the second Tuesday in the month”.

## See Also

### Constants

static var era: CFCalendarUnit

Specifies the era unit.

static var year: CFCalendarUnit

Specifies the year unit.

static var month: CFCalendarUnit

Specifies the month unit.

static var day: CFCalendarUnit

Specifies the day unit.

static var hour: CFCalendarUnit

Specifies the hour unit.

static var minute: CFCalendarUnit

Specifies the minute unit.

static var second: CFCalendarUnit

Specifies the second unit.

static var week: CFCalendarUnit

Specifies the week unit.

Deprecated

static var weekday: CFCalendarUnit

Specifies the weekday unit.

static var quarter: CFCalendarUnit

Specifies the quarter-year unit.

static var weekOfMonth: CFCalendarUnit

Specifies the original week of a month calendar unit.

static var weekOfYear: CFCalendarUnit

Specifies the original week of the year calendar unit.

static var yearForWeekOfYear: CFCalendarUnit

Specifies the relative year for a week within a year calendar unit.

