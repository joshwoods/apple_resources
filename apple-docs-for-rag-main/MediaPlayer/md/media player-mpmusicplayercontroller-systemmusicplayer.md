

- Media Player
- MPMusicPlayerController
-  systemMusicPlayer 

Type Property

# systemMusicPlayer

Returns the system music player, which controls the Music app’s state.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+tvOS 14.0+visionOS 1.0+

``` source
class var systemMusicPlayer: any MPMusicPlayerController & MPSystemMusicPlayerController { get }
```

## Return Value

The system music player.

## Discussion

The System music player employs the Music app on your behalf. On instantiation, it takes on the current Music app state and controls that state as your app runs. Specifically, the shared state includes the following:

- Repeat mode (see MPMusicRepeatMode)

- Shuffle mode (see MPMusicShuffleMode)

- Now-playing item (see nowPlayingItem)

- Playback state (see playbackState)

Other aspects of the Music app’s state aren’t shared. Music that’s playing continues to play when your app moves to the background.

## See Also

### Getting a music player

class var applicationMusicPlayer: MPMusicPlayerController

Returns the application music player.

class var applicationQueuePlayer: MPMusicPlayerApplicationController

Returns the application queue music player.

