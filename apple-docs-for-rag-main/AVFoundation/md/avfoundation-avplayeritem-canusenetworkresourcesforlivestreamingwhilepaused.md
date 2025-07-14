

- AVFoundation
- AVPlayerItem
-  canUseNetworkResourcesForLiveStreamingWhilePaused 

Instance Property

# canUseNetworkResourcesForLiveStreamingWhilePaused

A Boolean value that indicates whether the player item can use network resources to keep the playback state up to date while paused.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
nonisolated
var canUseNetworkResourcesForLiveStreamingWhilePaused: Bool { get set }
```

## Discussion

For live streaming content, the player item may need to use extra networking and power resources to keep playback state up to date when paused. For example, when this property is set to true, the seekableTimeRanges property will be periodically updated to reflect the current state of the live stream.

To minimize power usage, avoid setting this property to `true` when you do not need playback state to stay up to date while paused.

## See Also

### Configuring Network Behavior

var preferredPeakBitRate: Double

The desired limit, in bits per second, of network bandwidth consumption for this item.

var preferredForwardBufferDuration: TimeInterval

The duration the player should buffer media from the network ahead of the playhead to guard against playback disruption.

