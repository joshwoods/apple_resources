

- Core Foundation
-  CFCalendarUnit 

Structure

# CFCalendarUnit

CFCalendarUnit constants are used to specify calendrical units, such as day or month, in various calendar calculations.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct CFCalendarUnit
```

## Topics

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

static var weekdayOrdinal: CFCalendarUnit

Specifies the ordinal weekday unit.

static var quarter: CFCalendarUnit

Specifies the quarter-year unit.

static var weekOfMonth: CFCalendarUnit

Specifies the original week of a month calendar unit.

static var weekOfYear: CFCalendarUnit

Specifies the original week of the year calendar unit.

static var yearForWeekOfYear: CFCalendarUnit

Specifies the relative year for a week within a year calendar unit.

### Initializers

init(rawValue: CFOptionFlags)

### Type Properties

static var dayOfYear: CFCalendarUnit

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

### Constants

Component Wrapping Options

The wrapping option specifies overflow behavior for calendar components in calendrical calculations

