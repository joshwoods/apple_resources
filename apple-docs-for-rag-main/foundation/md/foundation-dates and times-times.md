

- Foundation
-  Dates and Times 

API Collection

# Dates and Times

Compare dates and times, and perform calendar and time zone calculations.

## Topics

### Date Representations

struct Date

A specific point in time, independent of any calendar or time zone.

struct DateInterval

The span of time between a specific start date and end date.

typealias TimeInterval

A number of seconds.

### Calendrical Calculations

struct DateComponents

A date or time specified in terms of units (such as year, month, day, hour, and minute) to be evaluated in a calendar system and time zone.

struct Calendar

A definition of the relationships between calendar units and absolute points in time, providing features for calculation and comparison of dates.

struct TimeZone

Information about standard time conventions associated with a specific geopolitical region.

### Date Formatting

class DateFormatter

A formatter that converts between dates and their textual representations.

class DateComponentsFormatter

A formatter that creates string representations of quantities of time.

class DateIntervalFormatter

A formatter that creates string representations of time intervals.

class ISO8601DateFormatter

A formatter that converts between dates and their ISO 8601 string representations.

### Internationalization

struct Locale

Information about linguistic, cultural, and technological conventions for use in formatting data for presentation.

## See Also

### Fundamentals

Numbers, Data, and Basic Values

Work with primitive values and other fundamental types used throughout Cocoa.

Strings and Text

Create and process strings of Unicode characters, use regular expressions to find patterns, and perform natural language analysis of text.

Collections

Use arrays, dictionaries, sets, and specialized collections to store and iterate groups of objects or values.

Units and Measurement

Label numeric quantities with physical dimensions to allow locale-aware formatting and conversion between related units.

Data Formatting

Convert numbers, dates, measurements, and other values to and from locale-aware string representations.

Filters and Sorting

Use predicates, expressions, and sort descriptors to examine elements in collections and other services.

