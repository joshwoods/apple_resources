

- Core Media
-  CMClockMakeHostTimeFromSystemUnits(\_:) 

Function

# CMClockMakeHostTimeFromSystemUnits(\_:)

Converts a host time from native units to a core media time structure.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMClockMakeHostTimeFromSystemUnits(_ hostTime: UInt64) -> CMTime
```

## Parameters 

`hostTime`  

The host time, in native units, to convert.

## Discussion

The return value has a large integer timescale (for example, nanoseconds). This function handles situations where the host time’s native units use a non-integer timescale.

In macOS, this function converts from the units of `mach_absolute_time`.

## See Also

### Accessing and Converting Time

func CMClockGetTime(CMClock) -> CMTime

Returns the current time from a clock.

func CMClockGetAnchorTime(CMClock, clockTimeOut: UnsafeMutablePointer&lt;CMTime>, referenceClockTimeOut: UnsafeMutablePointer&lt;CMTime>) -> OSStatus

Returns the current time from a clock and the matching time from the clock’s reference clock.

func CMClockConvertHostTimeToSystemUnits(CMTime) -> UInt64

Converts a host time from a core media time structure to the host time’s native units.

