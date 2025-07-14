

- Core Media
-  CMSyncConvertTime(\_:from:to:) 

Function

# CMSyncConvertTime(\_:from:to:)

Converts a time from one timebase or clock to another timebase or clock.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMSyncConvertTime(
    _ time: CMTime,
    from fromClockOrTimebase: CMClockOrTimebase,
    to toClockOrTimebase: CMClockOrTimebase
) -> CMTime
```

## Discussion

If both have a common host, the function syncs the clock or timebase based on the rates in the common tree rooted in that host.

If they have different host clocks (or are both clocks), this calculation also compensates for measured drift between the clocks. To convert to or from host time, pass `CMClockGetHostTimeClock`() as the appropriate argument.

## See Also

### Getting and Syncing Time

func CMSyncGetTime(CMClockOrTimebase) -> CMTime

Returns the time from a clock or timebase.

func CMSyncGetRelativeRate(CMClockOrTimebase, relativeTo: CMClockOrTimebase) -> Float64

Returns the relative rate of one timebase or clock relative to another timebase or clock.

func CMSyncGetRelativeRateAndAnchorTime(CMClockOrTimebase, relativeTo: CMClockOrTimebase, relativeRateOut: UnsafeMutablePointer&lt;Float64>?, anchorTimeOut: UnsafeMutablePointer&lt;CMTime>?, relativeToAnchorTimeOut: UnsafeMutablePointer&lt;CMTime>?) -> OSStatus

Returns the relative rate of one timebase or clock relative to another timebase or clock and the times of each timebase or clock at which the relative rate went into effect.

