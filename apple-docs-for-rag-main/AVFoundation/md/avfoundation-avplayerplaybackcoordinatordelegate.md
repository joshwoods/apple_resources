

- AVFoundation
-  AVPlayerPlaybackCoordinatorDelegate 

Protocol

# AVPlayerPlaybackCoordinatorDelegate

A protocol that defines the methods to implement to participate in playback coordination.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
protocol AVPlayerPlaybackCoordinatorDelegate : NSObjectProtocol, Sendable
```

## Topics

### Identifying Items

func playbackCoordinator(AVPlayerPlaybackCoordinator, identifierFor: AVPlayerItem) -> String

Returns an identifier for a player item.

### Retrieving Interstitial Time Ranges

func playbackCoordinator(AVPlayerPlaybackCoordinator, interstitialTimeRangesFor: AVPlayerItem) -> [NSValue]

Asks the delegate for time ranges in a player item that don’t correspond to the primary content.

## Relationships

### Inherits From

- NSObjectProtocol
- Sendable

## See Also

### Configuring the Delegate

var delegate: (any AVPlayerPlaybackCoordinatorDelegate)?

A delegate object for the playback coordinator.

