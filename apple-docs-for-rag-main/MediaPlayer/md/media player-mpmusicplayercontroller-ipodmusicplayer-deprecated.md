

- Media Player
- MPMusicPlayerController
-  iPodMusicPlayer Deprecated

Type Property

# iPodMusicPlayer

Returns the iPod music player, which controls the iPod app’s state.

iOS 3.0–8.0DeprecatediPadOS 3.0–8.0DeprecatedMac Catalyst 13.1–13.1DeprecatedvisionOS 1.0–1.0Deprecated

``` source
class var iPodMusicPlayer: MPMusicPlayerController { get }
```

Deprecated

The iPod app was renamed. Use the systemMusicPlayer method instead.

## Return Value

The iPod music player.

## Discussion

The iPod music player employs the iPod app on your behalf. On instantiation, it takes on the current iPod app state and controls that state as your app runs. Specifically, the shared state includes the following:

- Repeat mode (see MPMusicRepeatMode)

- Shuffle mode (see MPMusicShuffleMode

- Now-playing item (see nowPlayingItem)

- Playback state (see playbackState)

Other aspects of iPod state, such as the on-the-go playlist, aren’t shared. Music that’s playing continues to play when your app moves to the background.

