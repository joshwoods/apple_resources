

- MusicKit
- MusicPlayer
-  MusicPlayer.Queue 

Class

# MusicPlayer.Queue

A representation of the playback queue for a music player.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 14.0+tvOS 15.0+visionOS 1.0+

``` source
class Queue
```

## Topics

### Structures

struct Entry

An entry for the playback queue of the music player.

### Initializers

init&lt;S>(S, startingAt: S.Element?)

Creates a playback queue with playback queue entries.

init(album: Album, startingAt: Track)

Creates a playback queue with an album and a specific track for the player to start playback.

convenience init(arrayLiteral: any PlayableMusicItem...)

Creates an instance initialized with the given elements.

init&lt;S, PlayableMusicItemType>(for: S, startingAt: S.Element?)

Creates a playback queue with playable music items.

init(playlist: Playlist, startingAt: Playlist.Entry)

Creates a playback queue with a playlist and a specific playlist entry for the player to start playback.

### Instance Properties

var currentEntry: MusicPlayer.Queue.Entry?

The currently active entry in the playback queue.

var objectWillChange: AnyPublisher&lt;Void, Never>

A publisher that emits before the object has changed.

### Instance Methods

func insert&lt;PlayableMusicItemType>(PlayableMusicItemType, position: MusicPlayer.Queue.EntryInsertionPosition) async throws

Inserts a playable music item into the playback queue.

func insert&lt;S, PlayableMusicItemType>(S, position: MusicPlayer.Queue.EntryInsertionPosition) async throws

Inserts playable music items into the playback queue.

func insert(MusicPlayer.Queue.Entry, position: MusicPlayer.Queue.EntryInsertionPosition) async throws

Inserts an entry into the playback queue.

func insert&lt;S>(S, position: MusicPlayer.Queue.EntryInsertionPosition) async throws

Inserts entries into the playback queue.

### Type Aliases

typealias ArrayLiteralElement

The type of the elements of an array literal.

typealias ObjectWillChangePublisher

The type of publisher that emits before the object has changed.

### Enumerations

enum EntryInsertionPosition

An enumeration for the various supported positions for inserting playable music items or entries in the playback queue.

### Default Implementations

Equatable Implementations

Hashable Implementations

## Relationships

### Inherited By

- ApplicationMusicPlayer.Queue

### Conforms To

- Copyable
- Equatable
- ExpressibleByArrayLiteral
- Hashable
- ObservableObject

