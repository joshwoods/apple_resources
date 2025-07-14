

- Core Foundation
-  CFGregorianUnits Deprecated

Structure

# CFGregorianUnits

Structure used to represent a time interval in Gregorian units.

iOS 2.0–8.0DeprecatediPadOS 2.0–8.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.4–10.10DeprecatedtvOS 9.0–9.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–2.0Deprecated

``` source
struct CFGregorianUnits
```

Deprecated

Use CFCalendar or NSCalendar API instead

## Overview

A CFGregorianUnits is used to represent arbitrary time *intervals* (to represent a point in time using Gregorian units, use a CFGregorianDate). Each field can take values up to the maximum possible for its data type. Negative values are also valid.

## Topics

### Initializers

init()

init(years: Int32, months: Int32, days: Int32, hours: Int32, minutes: Int32, seconds: Double)

### Instance Properties

var days: Int32

var hours: Int32

var minutes: Int32

var months: Int32

var seconds: Double

var years: Int32

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Data Types

typealias CFAbsoluteTime

Type used to represent a specific point in time relative to the absolute reference date of 1 Jan 2001 00:00:00 GMT.

struct CFGregorianDate

Structure used to represent a point in time using the Gregorian calendar.

Deprecated

typealias CFTimeInterval

Type used to represent elapsed time in seconds.

