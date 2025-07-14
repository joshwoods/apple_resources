

- Core Foundation
-  CFGregorianDate Deprecated

Structure

# CFGregorianDate

Structure used to represent a point in time using the Gregorian calendar.

iOS 2.0–8.0DeprecatediPadOS 2.0–8.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.4–10.10DeprecatedtvOS 9.0–9.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–2.0Deprecated

``` source
struct CFGregorianDate
```

Deprecated

Use CFCalendar or NSCalendar API instead

## Overview

CFGregorianDate is implemented using the smallest data type appropriate for the range of possible values. For example, there are only 12 months in the Gregorian year, so there is no need to use an integer type larger than 8 bits. To represent a time interval in Gregorian units, use a CFGregorianUnits.

The month and day units are 1-based: the index for January is 1, and the index for the first day of the month is 1.

## Topics

### Initializers

init()

init(year: Int32, month: Int8, day: Int8, hour: Int8, minute: Int8, second: Double)

### Instance Properties

var day: Int8

var hour: Int8

var minute: Int8

var month: Int8

var second: Double

var year: Int32

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Data Types

typealias CFAbsoluteTime

Type used to represent a specific point in time relative to the absolute reference date of 1 Jan 2001 00:00:00 GMT.

struct CFGregorianUnits

Structure used to represent a time interval in Gregorian units.

Deprecated

typealias CFTimeInterval

Type used to represent elapsed time in seconds.

