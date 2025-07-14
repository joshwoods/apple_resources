

- Core Foundation
-  CFGregorianDateIsValid(\_:\_:) Deprecated

Function

# CFGregorianDateIsValid(\_:\_:)

Checks the specified fields of a CFGregorianDate structure for valid values.

iOS 2.0–8.0DeprecatediPadOS 2.0–8.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.4–10.10DeprecatedtvOS 9.0–9.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–2.0Deprecated

``` source
func CFGregorianDateIsValid(
    _ gdate: CFGregorianDate,
    _ unitFlags: CFOptionFlags
) -> Bool
```

Deprecated

Use CFCalendar or NSCalendar API instead

## Parameters 

`gdate`  

The CFGregorianDate structure whose fields to validate.

`unitFlags`  

A mask that specifies which Gregorian unit fields to validate. See CFGregorianUnitFlags for a list of values from which to construct the mask.

## Return Value

`true` if the specified fields are valid, otherwise `false`.

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

