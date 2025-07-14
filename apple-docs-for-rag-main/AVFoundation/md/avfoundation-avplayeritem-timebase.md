

- AVFoundation
- AVPlayerItem
-  timebase 

Instance Property

# timebase

The timebase information for the item.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
nonisolated
var timebase: CMTimebase? { get }
```

## Discussion

The system uses timebase information to synchronize playback of the current item with the host clock. You can use this property to access the timebase information, but you can’t use it to set the time or the rate of playback.

If you need to respond to changes in the effective playback rate, listen for kCMTimebaseNotification_EffectiveRateChanged notifications that the player item’s timebase posts. These notifications announce when the effective playback rate changes, which includes any compensation necessary for drifting behaviors of audio output hardware.

## See Also

### Accessing Timing Information

func currentTime() -> CMTime

Returns the current time of the item.

func currentDate() -> Date?

Returns the current time of the item as a date.

var duration: CMTime

The duration of the item.

