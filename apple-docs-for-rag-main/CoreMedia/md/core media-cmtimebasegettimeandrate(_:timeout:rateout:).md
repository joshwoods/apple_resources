

- Core Media
-  CMTimebaseGetTimeAndRate(\_:timeOut:rateOut:) 

Function

# CMTimebaseGetTimeAndRate(\_:timeOut:rateOut:)

Returns the current time and rate of a timebase.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMTimebaseGetTimeAndRate(
    _ timebase: CMTimebase,
    timeOut: UnsafeMutablePointer?,
    rateOut: UnsafeMutablePointer?
) -> OSStatus
```

## Discussion

You can use this function to take a consistent snapshot of the two values, avoiding possible inconsistencies due to external changes between retrieval of time and rate.

## See Also

### Getting and Setting Time

func CMTimebaseGetTime(CMTimebase) -> CMTime

Returns the current time from a timebase.

func CMTimebaseGetTimeWithTimeScale(CMTimebase, timescale: CMTimeScale, method: CMTimeRoundingMethod) -> CMTime

Returns the current time from a timebase in the specified timescale.

func CMTimebaseSetTime(CMTimebase, time: CMTime) -> OSStatus

Sets the current time of a timebase.

func CMTimebaseSetSourceClock(CMTimebase, CMClock) -> OSStatus

Sets the source clock of a timebase.

func CMTimebaseSetSourceTimebase(CMTimebase, CMTimebase) -> OSStatus

Sets the source timebase of a timebase.

func CMTimebaseSetAnchorTime(CMTimebase, timebaseTime: CMTime, immediateSourceTime: CMTime) -> OSStatus

Sets the time of a timebase at a particular host time.

