

- Core Foundation
- CFDateFormatter
-  Date Formatter Property Keys 

API Collection

# Date Formatter Property Keys

Keys used in key-value pairs to discover and specify the value of date formatter properties—used in conjunction with CFDateFormatterCopyProperty(_:_:) and CFDateFormatterSetProperty(_:_:_:).

## Overview

The values for these keys are all CFType objects. The specific types for each key are specified above.

## Topics

### Constants

static let isLenient: CFDateFormatterKey!

Specifies the lenient property, a CFBoolean object where a true value indicates that the parsing of strings into date or absolute time values will be fuzzy.

static let timeZone: CFDateFormatterKey!

Specifies the time zone property, a CFTimeZone object.

static let calendarName: CFDateFormatterKey!

Specifies the calendar name, a CFString object.

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

static let standaloneMonthSymbols: CFDateFormatterKey!

Specifies the standalone month symbols property, a CFArray of CFString objects.

static let shortStandaloneMonthSymbols: CFDateFormatterKey!

Specifies the short standalone month symbols property, a CFArray of CFString objects.

static let veryShortStandaloneMonthSymbols: CFDateFormatterKey!

Specifies the very short standalone month symbols property, a CFArray of CFString objects.

static let veryShortWeekdaySymbols: CFDateFormatterKey!

Specifies the very short weekday symbols property, a CFArray of CFString objects.

static let standaloneWeekdaySymbols: CFDateFormatterKey!

Specifies the standalone weekday symbols property, a CFArray of CFString objects.

static let shortStandaloneWeekdaySymbols: CFDateFormatterKey!

Specifies the short standalone weekday symbols property, a CFArray of CFString objects.

static let veryShortStandaloneWeekdaySymbols: CFDateFormatterKey!

Specifies the very short standalone weekday symbols property, a CFArray of CFString objects.

static let quarterSymbols: CFDateFormatterKey!

Specifies the quarter symbols property, a CFArray of CFString objects.

static let shortQuarterSymbols: CFDateFormatterKey!

Specifies the short quarter symbols property, a CFArray of CFString objects.

static let standaloneQuarterSymbols: CFDateFormatterKey!

Specifies the standalone quarter symbols property, a CFArray of CFString objects.

static let shortStandaloneQuarterSymbols: CFDateFormatterKey!

Specifies the short standalone quarter symbols property, a CFArray of CFString objects.

static let gregorianStartDate: CFDateFormatterKey!

Specifies the Gregorian start date property, a CFDate object.

static let doesRelativeDateFormattingKey: CFDateFormatterKey!

Specifies the relative date formatting property, a CFBoolean object.

## See Also

### Constants

Date Formatter Styles

Predefined date and time format styles.

Calendar Names

Calendar names used by CFDateFormatter.

