

- Core Media
-  CMTimebaseGetEffectiveRate(\_:) 

Function

# CMTimebaseGetEffectiveRate(\_:)

Returns the effective rate of a timebase, which combines its rate with the rates of all its host timebases.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMTimebaseGetEffectiveRate(_ timebase: CMTimebase) -> Float64
```

## Discussion

Calling `CMTimebaseGetEffectiveRate(timebase)` is equivalent to calling `CMSyncGetRelativeRate(timebase, CMTimebaseGetUltimateMasterClock(timebase))`.

## See Also

### Getting and Setting the Time Rate

func CMTimebaseGetRate(CMTimebase) -> Float64

Returns the current rate of a timebase.

func CMTimebaseSetRate(CMTimebase, rate: Float64) -> OSStatus

Sets the rate of a timebase.

func CMTimebaseSetRateAndAnchorTime(CMTimebase, rate: Float64, anchorTime: CMTime, immediateSourceTime: CMTime) -> OSStatus

Sets the time of a timebase at a particular host time, and changes the rate at exactly that time.

