

- AVFoundation
- AVPlayerItem
-  duration 

Instance Property

# duration

The duration of the item.

iOS 4.3+iPadOS 4.3+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
nonisolated
var duration: CMTime { get }
```

## Discussion

This property indicates the duration of the item, not considering either its forwardPlaybackEndTime or reversePlaybackEndTime.

The system reports the value of this property as indefinite until it loads the duration of the underlying asset. There are two ways to make sure you don’t access the value of duration until the system makes it available:

- Wait until the status of the player item is AVPlayerItem.Status.readyToPlay.

- Register for key-value observation of the property and request the initial value. If the system reports the initial value as indefinite, wait for the player item to notify you when duration becomes available.

Note

The value of duration may remain indefinite for live streams.

## See Also

### Accessing Timing Information

func currentTime() -> CMTime

Returns the current time of the item.

func currentDate() -> Date?

Returns the current time of the item as a date.

var timebase: CMTimebase?

The timebase information for the item.

