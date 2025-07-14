

- Core Foundation
-  CFAbsoluteTimeGetDayOfYear(\_:\_:) Deprecated

Function

# CFAbsoluteTimeGetDayOfYear(\_:\_:)

Returns an integer representing the day of the year indicated by the specified absolute time.

iOS 2.0–8.0DeprecatediPadOS 2.0–8.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.4–10.10DeprecatedtvOS 9.0–9.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–2.0Deprecated

``` source
func CFAbsoluteTimeGetDayOfYear(
    _ at: CFAbsoluteTime,
    _ tz: CFTimeZone!
) -> Int32
```

Deprecated

Use CFCalendar or NSCalendar API instead

## Parameters 

`at`  

The absolute time to convert.

`tz`  

The time zone to use for time correction. Pass `NULL` for GMT.

## Return Value

An integer (`1-366`) representing the day of the year specified by `at`.

## See Also

### Core Foundation Time Utilities Miscellaneous Functions

func CFAbsoluteTimeAddGregorianUnits(CFAbsoluteTime, CFTimeZone!, CFGregorianUnits) -> CFAbsoluteTime

Adds a time interval, expressed as Gregorian units, to a given absolute time.

Deprecated

func CFAbsoluteTimeGetCurrent() -> CFAbsoluteTime

Returns the current system absolute time.

func CFAbsoluteTimeGetDayOfWeek(CFAbsoluteTime, CFTimeZone!) -> Int32

Returns an integer representing the day of the week indicated by the specified absolute time.

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

