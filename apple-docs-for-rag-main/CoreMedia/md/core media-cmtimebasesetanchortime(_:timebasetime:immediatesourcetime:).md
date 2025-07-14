

- Core Media
-  CMTimebaseSetAnchorTime(\_:timebaseTime:immediateSourceTime:) 

Function

# CMTimebaseSetAnchorTime(\_:timebaseTime:immediateSourceTime:)

Sets the time of a timebase at a particular host time.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMTimebaseSetAnchorTime(
    _ timebase: CMTimebase,
    timebaseTime: CMTime,
    immediateSourceTime: CMTime
) -> OSStatus
```

## Discussion

The system interpolates `CMTimebaseGetTime`’s results from the anchor time.

`CMTimebaseSetTime(timebase, time)` is equivalent to calling `CMTimebaseSetAnchorTime(timebase, time, CMSyncGetTime(CMTimebaseCopySource(timebase)))`.

## See Also

### Getting and Setting Time

func CMTimebaseGetTime(CMTimebase) -> CMTime

Returns the current time from a timebase.

func CMTimebaseGetTimeWithTimeScale(CMTimebase, timescale: CMTimeScale, method: CMTimeRoundingMethod) -> CMTime

Returns the current time from a timebase in the specified timescale.

func CMTimebaseGetTimeAndRate(CMTimebase, timeOut: UnsafeMutablePointer&lt;CMTime>?, rateOut: UnsafeMutablePointer&lt;Float64>?) -> OSStatus

Returns the current time and rate of a timebase.

func CMTimebaseSetTime(CMTimebase, time: CMTime) -> OSStatus

Sets the current time of a timebase.

func CMTimebaseSetSourceClock(CMTimebase, CMClock) -> OSStatus

Sets the source clock of a timebase.

func CMTimebaseSetSourceTimebase(CMTimebase, CMTimebase) -> OSStatus

Sets the source timebase of a timebase.

