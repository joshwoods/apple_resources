

- Media Player
- MPMusicPlayerController
-  volume Deprecated

Instance Property

# volume

The audio playback volume for the music player, in the range from `0.0` (silent) through `1.0` (maximum volume).

visionOS 1.0–1.0Deprecated

``` source
var volume: Float { get set }
```

Deprecated

To provide UI for adjusting system playback volume, use the MPVolumeView class, which provides media playback controls that iOS users expect and whose appearance you can customize.

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

enum MPMusicRepeatMode

The repeat modes for the media player.

enum MPMusicShuffleMode

The shuffle modes for the media player.

