

- Core Media
-  CMTimebaseGetRate(\_:) 

Function

# CMTimebaseGetRate(\_:)

Returns the current rate of a timebase.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMTimebaseGetRate(_ timebase: CMTimebase) -> Float64
```

## Discussion

This is the rate relative to its immediate host clock or timebase. For example, if a timebase is running at twice the rate of its host, its rate is 2.0.

## See Also

### Getting and Setting the Time Rate

func CMTimebaseGetEffectiveRate(CMTimebase) -> Float64

Returns the effective rate of a timebase, which combines its rate with the rates of all its host timebases.

func CMTimebaseSetRate(CMTimebase, rate: Float64) -> OSStatus

Sets the rate of a timebase.

func CMTimebaseSetRateAndAnchorTime(CMTimebase, rate: Float64, anchorTime: CMTime, immediateSourceTime: CMTime) -> OSStatus

Sets the time of a timebase at a particular host time, and changes the rate at exactly that time.

