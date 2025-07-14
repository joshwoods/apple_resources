

- Core Foundation
- CFLocale
-  Locale Calendar Identifiers 

API Collection

# Locale Calendar Identifiers

Predefined locale keys used to get calendar values—values for `kCFLocaleCalendarIdentifier`.

## Overview

Locale objects use key-value pairs to store property values. Use the CFLocaleGetValue(_:_:) function to get the value of a specific property listed above.

## Topics

### Constants

static let gregorianCalendar: CFCalendarIdentifier!

The name of the calendar currently supported by the calendarName property.

static let buddhistCalendar: CFCalendarIdentifier!

Specifies the Buddhist calendar.

static let chineseCalendar: CFCalendarIdentifier!

Specifies the Chinese calendar.

static let hebrewCalendar: CFCalendarIdentifier!

Specifies the Hebrew calendar.

static let islamicCalendar: CFCalendarIdentifier!

Specifies the Islamic calendar.

static let islamicCivilCalendar: CFCalendarIdentifier!

Specifies the Islamic tabular calendar with Friday (civil) origin.

static let islamicTabularCalendar: CFCalendarIdentifier!

Specifies the Islamic tabular calendar with Thursday (astronomical) origin.

static let islamicUmmAlQuraCalendar: CFCalendarIdentifier!

Specifies the Islamic Umm Al Qura calendar.

static let japaneseCalendar: CFCalendarIdentifier!

Specifies the Japanese calendar.

static let republicOfChinaCalendar: CFCalendarIdentifier!

Specifies the calendar for the Republic of China.

static let persianCalendar: CFCalendarIdentifier!

Specifies the Persian calendar.

static let indianCalendar: CFCalendarIdentifier!

Specifies the Indian calendar.

static let cfiso8601Calendar: CFCalendarIdentifier!

Specifies the ISO 8601 calendar.

## See Also

### Constants

enum CFLocaleLanguageDirection

These constants describe the text direction for a language. They are returned by the functions CFLocaleGetLanguageCharacterDirection(_:) and CFLocaleGetLanguageLineDirection(_:).

Locale Property Keys

Predefined locale keys used to get property values.

Locale Change Notification

Identifier for notification sent if the current locale changes.

