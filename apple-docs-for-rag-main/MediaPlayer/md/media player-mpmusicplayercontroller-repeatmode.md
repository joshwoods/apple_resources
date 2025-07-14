

- Media Player
- MPMusicPlayerController
-  repeatMode 

Instance Property

# repeatMode

The current repeat mode of the music player.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+tvOS 14.0+visionOS 1.0+

``` source
var repeatMode: MPMusicRepeatMode { get set }
```

## Discussion

For the available repeat modes, see MPMusicRepeatMode. If not explicitly set, `repeatMode` defaults to MPMusicRepeatMode.default.

## See Also

### Managing playback mode and state

var nowPlayingItem: MPMediaItem?

The currently-playing media item, or the media item in a queue that you designated to begin playback with.

var indexOfNowPlayingItem: Int

The index of the now playing item in the current playback queue.

var playbackState: MPMusicPlaybackState

The current playback state of the music player.

var shuffleMode: MPMusicShuffleMode

The current shuffle mode of the music player.

enum MPMusicPlaybackState

The music player playback state modes.

enum MPMusicRepeatMode

The repeat modes for the media player.

enum MPMusicShuffleMode

The shuffle modes for the media player.

var volume: Float

The audio playback volume for the music player, in the range from `0.0` (silent) through `1.0` (maximum volume).

Deprecated

