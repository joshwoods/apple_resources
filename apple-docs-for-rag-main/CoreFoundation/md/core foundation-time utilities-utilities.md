

- Core Foundation
-  Time Utilities 

API Collection

# Time Utilities

## Overview

Core Foundation measures time in units of seconds. The base data type is the CFTimeInterval, which measures the difference in seconds between two times. Fixed times, or dates, are defined by the CFAbsoluteTime data type, which measures the time interval between a particular date and the absolute reference date of Jan 1 2001 00:00:00 GMT.

The CFGregorianDate structure represents absolute times in terms of the Gregorian calendar. Functions such as CFAbsoluteTimeGetGregorianDate(_:_:) use a CFTimeZone object to obtain the local time in a particular time zone.

The CFDate opaque type wraps an absolute time into a CFTypeRef-base object, allowing you to put time objects into collections and property lists and to be handled by other object-oriented parts of Core Foundation.

## Topics

### Core Foundation Time Utilities Miscellaneous Functions

func CFAbsoluteTimeAddGregorianUnits(CFAbsoluteTime, CFTimeZone!, CFGregorianUnits) -> CFAbsoluteTime

Adds a time interval, expressed as Gregorian units, to a given absolute time.

Deprecated

func CFAbsoluteTimeGetCurrent() -> CFAbsoluteTime

Returns the current system absolute time.

func CFAbsoluteTimeGetDayOfWeek(CFAbsoluteTime, CFTimeZone!) -> Int32

Returns an integer representing the day of the week indicated by the specified absolute time.

Deprecated

func CFAbsoluteTimeGetDayOfYear(CFAbsoluteTime, CFTimeZone!) -> Int32

Returns an integer representing the day of the year indicated by the specified absolute time.

Deprecated

func CFAbsoluteTimeGetDifferenceAsGregorianUnits(CFAbsoluteTime, CFAbsoluteTime, CFTimeZone!, CFOptionFlags) -> CFGregorianUnits

Computes the time difference between two specified absolute times and returns the result as an interval in Gregorian units.

Deprecated

func CFAbsoluteTimeGetGregorianDate(CFAbsoluteTime, CFTimeZone!) -> CFGregorianDate

Converts an absolute time value into a Gregorian date.

Deprecated

func CFAbsoluteTimeGetWeekOfYear(CFAbsoluteTime, CFTimeZone!) -> Int32

Returns an integer representing the week of the year indicated by the specified absolute time.

Deprecated

func CFGregorianDateGetAbsoluteTime(CFGregorianDate, CFTimeZone!) -> CFAbsoluteTime

Converts a Gregorian date value into an absolute time value.

Deprecated

func CFGregorianDateIsValid(CFGregorianDate, CFOptionFlags) -> Bool

Checks the specified fields of a CFGregorianDate structure for valid values.

Deprecated

### Data Types

typealias CFAbsoluteTime

Type used to represent a specific point in time relative to the absolute reference date of 1 Jan 2001 00:00:00 GMT.

struct CFGregorianDate

Structure used to represent a point in time using the Gregorian calendar.

Deprecated

struct CFGregorianUnits

Structure used to represent a time interval in Gregorian units.

Deprecated

typealias CFTimeInterval

Type used to represent elapsed time in seconds.

### Constants

struct CFGregorianUnitFlags

These option flags are used as a mask to indicate a specific set of fields in the CFGregorianDate or CFGregorianUnits structures.

Predefined Time Interval Values

Time intervals between the absolute reference date and certain other dates.

## See Also

### Related Documentation

Date and Time Programming Guide for Core Foundation

### Utilities

Base Utilities

Byte-Order Utilities

Core Foundation URL Access Utilities

Preferences Utilities

Socket Name Server Utilities

