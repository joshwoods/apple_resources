

- Core Foundation
-  CFAbsoluteTime 

Type Alias

# CFAbsoluteTime

Type used to represent a specific point in time relative to the absolute reference date of 1 Jan 2001 00:00:00 GMT.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
typealias CFAbsoluteTime = CFTimeInterval
```

## Discussion

Absolute time is measured by the number of seconds between the reference date and the specified date. Negative values indicate dates/times before the reference date. Positive values indicate dates/times after the reference date.

## See Also

### Data Types

struct CFGregorianDate

Structure used to represent a point in time using the Gregorian calendar.

Deprecated

struct CFGregorianUnits

Structure used to represent a time interval in Gregorian units.

Deprecated

typealias CFTimeInterval

Type used to represent elapsed time in seconds.

