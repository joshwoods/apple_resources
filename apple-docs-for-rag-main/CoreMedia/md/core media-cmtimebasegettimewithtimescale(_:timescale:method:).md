

- Core Media
-  CMTimebaseGetTimeWithTimeScale(\_:timescale:method:) 

Function

# CMTimebaseGetTimeWithTimeScale(\_:timescale:method:)

Returns the current time from a timebase in the specified timescale.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMTimebaseGetTimeWithTimeScale(
    _ timebase: CMTimebase,
    timescale: CMTimeScale,
    method: CMTimeRoundingMethod
) -> CMTime
```

## See Also

### Getting and Setting Time

func CMTimebaseGetTime(CMTimebase) -> CMTime

Returns the current time from a timebase.

func CMTimebaseGetTimeAndRate(CMTimebase, timeOut: UnsafeMutablePointer&lt;CMTime>?, rateOut: UnsafeMutablePointer&lt;Float64>?) -> OSStatus

Returns the current time and rate of a timebase.

func CMTimebaseSetTime(CMTimebase, time: CMTime) -> OSStatus

Sets the current time of a timebase.

func CMTimebaseSetSourceClock(CMTimebase, CMClock) -> OSStatus

Sets the source clock of a timebase.

func CMTimebaseSetSourceTimebase(CMTimebase, CMTimebase) -> OSStatus

Sets the source timebase of a timebase.

func CMTimebaseSetAnchorTime(CMTimebase, timebaseTime: CMTime, immediateSourceTime: CMTime) -> OSStatus

Sets the time of a timebase at a particular host time.

