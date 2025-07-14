

- MusicKit
- ApplicationMusicPlayer
-  ApplicationMusicPlayer.Queue 

Class

# ApplicationMusicPlayer.Queue

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 14.0+tvOS 15.0+visionOS 1.0+

``` source
class Queue
```

## Topics

### Structures

struct Entries

### Initializers

init&lt;S>(S, startingAt: S.Element?)

Creates a playback queue with playback queue entries.

init(album: Album, startingAt: Track)

Creates a playback queue with an album and a specific track for the player to start playback.

init(arrayLiteral: any PlayableMusicItem...)

init&lt;S, PlayableMusicItemType>(for: S, startingAt: S.Element?)

Creates a playback queue with playable music items.

init(playlist: Playlist, startingAt: Playlist.Entry)

Creates a playback queue with a playlist and a specific playlist entry for the player to start playback.

### Instance Properties

var entries: ApplicationMusicPlayer.Queue.Entries

## Relationships

### Inherits From

- MusicPlayer.Queue

### Conforms To

- Equatable
- ExpressibleByArrayLiteral
- Hashable
- ObservableObject

