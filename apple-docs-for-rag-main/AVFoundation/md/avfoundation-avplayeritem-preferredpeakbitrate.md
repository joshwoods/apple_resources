

- AVFoundation
- AVPlayerItem
-  preferredPeakBitRate 

Instance Property

# preferredPeakBitRate

The desired limit, in bits per second, of network bandwidth consumption for this item.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
nonisolated
var preferredPeakBitRate: Double { get set }
```

## Discussion

Set `preferredPeakBitRate` to nonzero to indicate that the player should attempt to limit item playback to that bit rate, expressed in bits per second.

If the system can’t lower network bandwidth consumption to meet the this value, it reduces it as much as possible while it continues to play the item.

## See Also

### Configuring Network Behavior

var preferredForwardBufferDuration: TimeInterval

The duration the player should buffer media from the network ahead of the playhead to guard against playback disruption.

var canUseNetworkResourcesForLiveStreamingWhilePaused: Bool

A Boolean value that indicates whether the player item can use network resources to keep the playback state up to date while paused.

