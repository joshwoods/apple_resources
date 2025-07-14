

- Core Foundation
- CFDateFormatterKey
-  calendarName 

Type Property

# calendarName

Specifies the calendar name, a CFString object.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
static let calendarName: CFDateFormatterKey!
```

## Discussion

With OS X version 10.3, gregorianCalendar is the only possible value. With OS X version 10.4, `kCFGregorianCalendar` and other calendar names are specified by CFLocale.

## See Also

### Constants

static let isLenient: CFDateFormatterKey!

Specifies the lenient property, a CFBoolean object where a true value indicates that the parsing of strings into date or absolute time values will be fuzzy.

static let timeZone: CFDateFormatterKey!

Specifies the time zone property, a CFTimeZone object.

static let defaultFormat: CFDateFormatterKey!

The original format string for the formatter (given the date & time style and locale specified at creation).

static let twoDigitStartDate: CFDateFormatterKey!

Specifies the property representing the date from which two-digit years start, a CFDate object.

static let defaultDate: CFDateFormatterKey!

Specifies the default date property, a CFDate object.

static let calendar: CFDateFormatterKey!

Specifies the calendar property, a CFCalendar object.

static let eraSymbols: CFDateFormatterKey!

Specifies the era symbols property, a CFArray of CFString objects.

static let monthSymbols: CFDateFormatterKey!

Specifies the month symbols property, a CFArray of CFString objects.

static let shortMonthSymbols: CFDateFormatterKey!

Specifies the short month symbols property, a CFArray of CFString objects.

static let weekdaySymbols: CFDateFormatterKey!

Specifies the weekday symbols property, a CFArray of CFString objects.

static let shortWeekdaySymbols: CFDateFormatterKey!

Specifies the short weekday symbols property, a CFArray of CFString objects.

static let amSymbol: CFDateFormatterKey!

Specifies the AM symbol property, a CFString object.

static let pmSymbol: CFDateFormatterKey!

Specifies the PM symbol property, a CFString object.

static let longEraSymbols: CFDateFormatterKey!

Specifies the long era symbols property, a CFArray of CFString objects.

static let veryShortMonthSymbols: CFDateFormatterKey!

Specifies the very short month symbols property, a CFArray of CFString objects.

