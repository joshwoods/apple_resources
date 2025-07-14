

- Core Foundation
-  CFAbsoluteTimeGetDifferenceAsGregorianUnits(\_:\_:\_:\_:) Deprecated

Function

# CFAbsoluteTimeGetDifferenceAsGregorianUnits(\_:\_:\_:\_:)

Computes the time difference between two specified absolute times and returns the result as an interval in Gregorian units.

iOS 2.0–8.0DeprecatediPadOS 2.0–8.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.4–10.10DeprecatedtvOS 9.0–9.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–2.0Deprecated

``` source
func CFAbsoluteTimeGetDifferenceAsGregorianUnits(
    _ at1: CFAbsoluteTime,
    _ at2: CFAbsoluteTime,
    _ tz: CFTimeZone!,
    _ unitFlags: CFOptionFlags
) -> CFGregorianUnits
```

Deprecated

Use CFCalendar or NSCalendar API instead

## Parameters 

`at1`  

An absolute time.

`at2`  

An absolute time.

`tz`  

The time zone to use for time correction. Pass `NULL` for GMT.

`unitFlags`  

A mask that specifies which Gregorian unit fields to use when converting the absolute time difference into a Gregorian interval. See CFGregorianUnitFlags for a list of values from which to construct the mask.

## Return Value

The difference between the specified absolute times (as `at1 - at2`—if `at1` is earlier than `at2`, the result is negative) expressed in the units specified by `unitFlags`.

## Discussion

The temporal difference is expressed as accurately as possible, given the units specified. For example, if you asked for the number of months and hours between 2:30pm on April 8 2005 and 5:45pm September 9 2005, the result would be 5 months and 27 hours.

The following example prints the number of hours and minutes between the current time (now) and the reference date (1 January 2001 00:00:00 GMT).

```
CFAbsoluteTime now = CFAbsoluteTimeGetCurrent ();

CFGregorianUnits units = CFAbsoluteTimeGetDifferenceAsGregorianUnits
    (now, 0, NULL, (kCFGregorianUnitsHours | kCFGregorianUnitsMinutes));

CFStringRef output = CFStringCreateWithFormat
    (NULL, 0, CFSTR("hours: %d; minutes: %d"), units.hours, units.minutes);
CFShow(output);
```

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

func CFAbsoluteTimeGetDayOfYear(CFAbsoluteTime, CFTimeZone!) -> Int32

Returns an integer representing the day of the year indicated by the specified absolute time.

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

