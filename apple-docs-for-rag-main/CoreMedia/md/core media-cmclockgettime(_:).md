

- Core Media
-  CMClockGetTime(\_:) 

Function

# CMClockGetTime(\_:)

Returns the current time from a clock.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMClockGetTime(_ clock: CMClock) -> CMTime
```

## Parameters 

`clock`  

The clock to retrieve the current time from.

## See Also

### Accessing and Converting Time

func CMClockGetAnchorTime(CMClock, clockTimeOut: UnsafeMutablePointer&lt;CMTime>, referenceClockTimeOut: UnsafeMutablePointer&lt;CMTime>) -> OSStatus

Returns the current time from a clock and the matching time from the clock’s reference clock.

func CMClockConvertHostTimeToSystemUnits(CMTime) -> UInt64

Converts a host time from a core media time structure to the host time’s native units.

func CMClockMakeHostTimeFromSystemUnits(UInt64) -> CMTime

Converts a host time from native units to a core media time structure.

