

- Core Media
-  CMClockConvertHostTimeToSystemUnits(\_:) 

Function

# CMClockConvertHostTimeToSystemUnits(\_:)

Converts a host time from a core media time structure to the host time’s native units.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMClockConvertHostTimeToSystemUnits(_ hostTime: CMTime) -> UInt64
```

## Parameters 

`hostTime`  

The host time to convert.

## Discussion

This function performs a scale conversion, not a clock conversion. It can be more accurate than CMTimeConvertScale(_:timescale:method:) because the system units may have a non-integer timescale.

In macOS, this function converts to the units of `mach_absolute_time`.

## See Also

### Accessing and Converting Time

func CMClockGetTime(CMClock) -> CMTime

Returns the current time from a clock.

func CMClockGetAnchorTime(CMClock, clockTimeOut: UnsafeMutablePointer&lt;CMTime>, referenceClockTimeOut: UnsafeMutablePointer&lt;CMTime>) -> OSStatus

Returns the current time from a clock and the matching time from the clock’s reference clock.

func CMClockMakeHostTimeFromSystemUnits(UInt64) -> CMTime

Converts a host time from native units to a core media time structure.

