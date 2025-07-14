

- Media Player
- MPMusicPlayerController
-  nowPlayingItem 

Instance Property

# nowPlayingItem

The currently-playing media item, or the media item in a queue that you designated to begin playback with.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+tvOS 14.0+visionOS 1.0+

``` source
@NSCopying
var nowPlayingItem: MPMediaItem? { get set }
```

## Discussion

To specify that playback should begin at a particular media item in the playback queue, set this property to that item while the music player is in a stopped or paused state.

If no media item is playing or designated to play, this property’s value is `nil`.

If you use the system music player and the user plays an item from another library using Home Sharing, the value of this property is nil.

## See Also

### Managing playback mode and state

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

var volume: Float

The audio playback volume for the music player, in the range from `0.0` (silent) through `1.0` (maximum volume).

Deprecated

