

- Core Media
-  CMSyncGetTime(\_:) 

Function

# CMSyncGetTime(\_:)

Returns the time from a clock or timebase.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMSyncGetTime(_ clockOrTimebase: CMClockOrTimebase) -> CMTime
```

## Discussion

`CMSyncGetTime` calls either CMClockGetTime(_:) or CMTimebaseGetTime(_:), as appropriate.

## See Also

### Getting and Syncing Time

func CMSyncGetRelativeRate(CMClockOrTimebase, relativeTo: CMClockOrTimebase) -> Float64

Returns the relative rate of one timebase or clock relative to another timebase or clock.

func CMSyncGetRelativeRateAndAnchorTime(CMClockOrTimebase, relativeTo: CMClockOrTimebase, relativeRateOut: UnsafeMutablePointer&lt;Float64>?, anchorTimeOut: UnsafeMutablePointer&lt;CMTime>?, relativeToAnchorTimeOut: UnsafeMutablePointer&lt;CMTime>?) -> OSStatus

Returns the relative rate of one timebase or clock relative to another timebase or clock and the times of each timebase or clock at which the relative rate went into effect.

func CMSyncConvertTime(CMTime, from: CMClockOrTimebase, to: CMClockOrTimebase) -> CMTime

Converts a time from one timebase or clock to another timebase or clock.

