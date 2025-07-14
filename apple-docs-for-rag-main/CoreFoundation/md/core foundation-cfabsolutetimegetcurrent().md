

- Core Foundation
-  CFAbsoluteTimeGetCurrent() 

Function

# CFAbsoluteTimeGetCurrent()

Returns the current system absolute time.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFAbsoluteTimeGetCurrent() -> CFAbsoluteTime
```

## Return Value

The current absolute time.

## Discussion

Absolute time is measured in seconds relative to the absolute reference date of Jan 1 2001 00:00:00 GMT. A positive value represents a date after the reference date, a negative value represents a date before it. For example, the absolute time `-32940326` is equivalent to December 16th, 1999 at 17:54:34. Repeated calls to this function do not guarantee monotonically increasing results. The system time may decrease due to synchronization with external time references or due to an explicit user change of the clock.

## See Also

### Core Foundation Time Utilities Miscellaneous Functions

func CFAbsoluteTimeAddGregorianUnits(CFAbsoluteTime, CFTimeZone!, CFGregorianUnits) -> CFAbsoluteTime

Adds a time interval, expressed as Gregorian units, to a given absolute time.

Deprecated

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

