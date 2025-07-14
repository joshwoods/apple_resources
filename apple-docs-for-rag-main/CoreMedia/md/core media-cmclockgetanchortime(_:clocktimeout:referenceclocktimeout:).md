

- Core Media
-  CMClockGetAnchorTime(\_:clockTimeOut:referenceClockTimeOut:) 

Function

# CMClockGetAnchorTime(\_:clockTimeOut:referenceClockTimeOut:)

Returns the current time from a clock and the matching time from the clock’s reference clock.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMClockGetAnchorTime(
    _ clock: CMClock,
    clockTimeOut: UnsafeMutablePointer,
    referenceClockTimeOut: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`clock`  

The clock to retrieve the current time from.

`clockTimeOut`  

On output, points to the current time.

`referenceClockTimeOut`  

On output, points to the reference clock time.

## Discussion

To make practical use of this, you may need to know what the clock’s reference clock is.

## See Also

### Accessing and Converting Time

func CMClockGetTime(CMClock) -> CMTime

Returns the current time from a clock.

func CMClockConvertHostTimeToSystemUnits(CMTime) -> UInt64

Converts a host time from a core media time structure to the host time’s native units.

func CMClockMakeHostTimeFromSystemUnits(UInt64) -> CMTime

Converts a host time from native units to a core media time structure.

