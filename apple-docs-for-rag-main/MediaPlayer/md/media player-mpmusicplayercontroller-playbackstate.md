

- Media Player
- MPMusicPlayerController
-  playbackState 

Instance Property

# playbackState

The current playback state of the music player.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+tvOS 14.0+visionOS 1.0+

``` source
var playbackState: MPMusicPlaybackState { get }
```

## Discussion

If you configure a music player as a system music player, the playback state matches the playback state of the built-in Music app. This is true whether the Music app is using the device Music library or a home shared library. Note, however, that when the Music app is using a home shared library, the music player’s nowPlayingItem property is `nil`.

For the available playback states, see MPMusicPlaybackState.

## See Also

### Managing playback mode and state

var nowPlayingItem: MPMediaItem?

The currently-playing media item, or the media item in a queue that you designated to begin playback with.

var indexOfNowPlayingItem: Int

The index of the now playing item in the current playback queue.

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

var volume: Float

The audio playback volume for the music player, in the range from `0.0` (silent) through `1.0` (maximum volume).

Deprecated

