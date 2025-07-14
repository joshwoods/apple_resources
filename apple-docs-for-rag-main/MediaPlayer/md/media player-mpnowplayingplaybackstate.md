

- Media Player
-  MPNowPlayingPlaybackState 

Enumeration

# MPNowPlayingPlaybackState

The playback state of the app.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.12.2+tvOS 11.0+visionOS 1.0+watchOS 5.0+

``` source
enum MPNowPlayingPlaybackState
```

## Topics

### Playback states

case unknown

The current state of the app is unknown.

case playing

The app is currently playing a media item.

case paused

The app is currently paused.

case stopped

The app has stopped playing.

case interrupted

The app has been interrupted during playback.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Setting the playback state in macOS

var playbackState: MPNowPlayingPlaybackState

The current playback state of the app.

