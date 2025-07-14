

- MusicKit
-  SystemMusicPlayer 

Class

# SystemMusicPlayer

An object your app uses to play music by controlling the Music app’s state.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 15.0+visionOS 1.0+

``` source
class SystemMusicPlayer
```

## Overview

The system music player employs the Music app on your behalf. When your app accesses the system music player for the first time, it assumes the current Music app state and controls it as your app runs. The shared state includes the following:

- Repeat mode (see MusicPlayer.RepeatMode)

- Shuffle mode (see MusicPlayer.ShuffleMode)

- Playback status (see `MusicPlayer/PlaybackStatus`)

The system music player doesn’t share other aspects of the Music app’s state. Music that’s playing continues to play when your app moves to the background.

## Topics

### Instance Properties

var queue: MusicPlayer.Queue

The playback queue for the system music player.

### Type Properties

static let shared: SystemMusicPlayer

The shared system music player, which controls the Music app’s state.

## Relationships

### Inherits From

- MusicPlayer

## See Also

### Playback

class ApplicationMusicPlayer

An object your app uses to play music in a way that doesn’t affect the Music app’s state.

class MusicPlayer

An object your app uses to play music.

protocol PlayableMusicItem

A set of properties that a music player uses to initiate playback for a music item.

struct PlayParameters

An opaque object that represents parameters to initiate playback of a playable music item using a music player.

