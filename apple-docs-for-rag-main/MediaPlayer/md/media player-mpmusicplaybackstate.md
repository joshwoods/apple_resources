

- Media Player
-  MPMusicPlaybackState 

Enumeration

# MPMusicPlaybackState

The music player playback state modes.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+tvOS 14.0+visionOS 1.0+

``` source
enum MPMusicPlaybackState
```

## Overview

You determine a music player’s state by checking the playbackState property. Depending on the property’s value, you can update your application’s user interface or take other appropriate action.

## Topics

### Constants

case stopped

The music player is stopped.

case playing

The music player is playing.

case paused

The music player is paused.

case interrupted

The music player has been interrupted, such as by an incoming phone call.

case seekingForward

The music player is seeking forward.

case seekingBackward

The music player is seeking backward.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Managing playback mode and state

var nowPlayingItem: MPMediaItem?

The currently-playing media item, or the media item in a queue that you designated to begin playback with.

var indexOfNowPlayingItem: Int

The index of the now playing item in the current playback queue.

var playbackState: MPMusicPlaybackState

The current playback state of the music player.

var repeatMode: MPMusicRepeatMode

The current repeat mode of the music player.

var shuffleMode: MPMusicShuffleMode

The current shuffle mode of the music player.

enum MPMusicRepeatMode

The repeat modes for the media player.

enum MPMusicShuffleMode

The shuffle modes for the media player.

var volume: Float

The audio playback volume for the music player, in the range from `0.0` (silent) through `1.0` (maximum volume).

Deprecated

