

- AVFoundation
- AVPlayerItem
-  preferredForwardBufferDuration 

Instance Property

# preferredForwardBufferDuration

The duration the player should buffer media from the network ahead of the playhead to guard against playback disruption.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
nonisolated
var preferredForwardBufferDuration: TimeInterval { get set }
```

## Discussion

This property defines the preferred forward buffer duration in seconds. If set to 0, the player will choose an appropriate level of buffering for most use cases. Setting this property to a low value will increase the chance that playback will stall and re-buffer, while setting it to a high value will increase demand on system resources.

## See Also

### Configuring Network Behavior

var preferredPeakBitRate: Double

The desired limit, in bits per second, of network bandwidth consumption for this item.

var canUseNetworkResourcesForLiveStreamingWhilePaused: Bool

A Boolean value that indicates whether the player item can use network resources to keep the playback state up to date while paused.

