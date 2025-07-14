

- AVFoundation
- AVPlayerItem
-  status 

Instance Property

# status

The status of the player item.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
nonisolated
var status: AVPlayerItem.Status { get }
```

## Mentioned in 

Controlling the transport behavior of a player

## Discussion

When a player item is created, its status is AVPlayerItem.Status.unknown, meaning its media hasn’t been loaded and has not yet been enqueued for playback. Associating a player item with an AVPlayer immediately begins enqueuing the item’s media and preparing it for playback. When the player item’s media has been loaded and is ready for use, its status will change to AVPlayerItem.Status.readyToPlay. You can observe this change using key-value observing.

For possible values, see AVPlayerItem.Status.

## See Also

### Determining Readiness

enum Status

The statuses for a player item.

var error: (any Error)?

The error that caused the player item to fail.

