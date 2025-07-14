

- AVFoundation
- AVPlayerPlaybackCoordinatorDelegate
-  playbackCoordinator(\_:interstitialTimeRangesFor:) 

Instance Method

# playbackCoordinator(\_:interstitialTimeRangesFor:)

Asks the delegate for time ranges in a player item that don’t correspond to the primary content.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 12.3+tvOS 15.4+visionOS 1.0+

``` source
optional func playbackCoordinator(
    _ coordinator: AVPlayerPlaybackCoordinator,
    interstitialTimeRangesFor playerItem: AVPlayerItem
) -> [NSValue]
```

## Parameters 

`coordinator`  

The object coordinating playback.

`playerItem`  

The player item for which to retrieve interstitial time ranges.

## Return Value

An array of NSValue objects that contain the interstitial time ranges.

## Discussion

Implementing this method enables the coordinator to synchronize playback between participants that have different interstitials stitched into the primary content timeline.

If you don’t implement this method, the coordinator assumes that the entire item corresponds to the primary content.

