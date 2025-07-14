

- MusicKit
-  PlayableMusicItem 

Protocol

# PlayableMusicItem

A set of properties that a music player uses to initiate playback for a music item.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 14.0+tvOS 15.0+visionOS 1.0+

``` source
protocol PlayableMusicItem : MusicItem
```

## Topics

### Instance Properties

var playParameters: PlayParameters?

The parameters to use to play the music item.

**Required**

## Relationships

### Inherits From

- MusicItem
- Sendable

### Conforming Types

- Album
- MusicPlayer.Queue.Entry.Item
- Playlist
- Playlist.Entry
- Playlist.Entry.Item
- RecentlyPlayedMusicItem
- Song
- Station
- Track

## See Also

### Playback

class ApplicationMusicPlayer

An object your app uses to play music in a way that doesn’t affect the Music app’s state.

class SystemMusicPlayer

An object your app uses to play music by controlling the Music app’s state.

class MusicPlayer

An object your app uses to play music.

struct PlayParameters

An opaque object that represents parameters to initiate playback of a playable music item using a music player.

