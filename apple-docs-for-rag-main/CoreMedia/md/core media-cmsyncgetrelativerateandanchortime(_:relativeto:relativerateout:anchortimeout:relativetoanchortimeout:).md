

- Core Media
-  CMSyncGetRelativeRateAndAnchorTime(\_:relativeTo:relativeRateOut:anchorTimeOut:relativeToAnchorTimeOut:) 

Function

# CMSyncGetRelativeRateAndAnchorTime(\_:relativeTo:relativeRateOut:anchorTimeOut:relativeToAnchorTimeOut:)

Returns the relative rate of one timebase or clock relative to another timebase or clock and the times of each timebase or clock at which the relative rate went into effect.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMSyncGetRelativeRateAndAnchorTime(
    _ ofClockOrTimebase: CMClockOrTimebase,
    relativeTo relativeToClockOrTimebase: CMClockOrTimebase,
    relativeRateOut outRelativeRate: UnsafeMutablePointer?,
    anchorTimeOut outOfClockOrTimebaseAnchorTime: UnsafeMutablePointer?,
    relativeToAnchorTimeOut outRelativeToClockOrTimebaseAnchorTime: UnsafeMutablePointer?
) -> OSStatus
```

## Discussion

If both have a common host, the function syncs the clock or timebase based on the rates in the common tree rooted in that host.

If they have different host clocks (or are both clocks), this calculation takes into account the measured drift between the two clocks, using host time as a pivot. The rate of a moving timebase relative to a stopped timebase is a NaN.

## See Also

### Getting and Syncing Time

func CMSyncGetTime(CMClockOrTimebase) -> CMTime

Returns the time from a clock or timebase.

func CMSyncGetRelativeRate(CMClockOrTimebase, relativeTo: CMClockOrTimebase) -> Float64

Returns the relative rate of one timebase or clock relative to another timebase or clock.

func CMSyncConvertTime(CMTime, from: CMClockOrTimebase, to: CMClockOrTimebase) -> CMTime

Converts a time from one timebase or clock to another timebase or clock.

