

- Media Player
-  MPMusicRepeatMode 

Enumeration

# MPMusicRepeatMode

The repeat modes for the media player.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+tvOS 14.0+visionOS 1.0+

``` source
enum MPMusicRepeatMode
```

## Topics

### Constants

case `default`

The user’s preferred repeat mode.

case none

The music player will not repeat the current song or playlist.

case one

The music player will repeat the current song.

case all

The music player will repeat the current playlist.

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

enum MPMusicPlaybackState

The music player playback state modes.

enum MPMusicShuffleMode

The shuffle modes for the media player.

var volume: Float

The audio playback volume for the music player, in the range from `0.0` (silent) through `1.0` (maximum volume).

Deprecated

