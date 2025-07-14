

- MusicKit
- MusicPlayer
- MusicPlayer.Queue
- MusicPlayer.Queue.Entry
-  MusicPlayer.Queue.Entry.Item 

Enumeration

# MusicPlayer.Queue.Entry.Item

An item that corresponds to an entry in the playback queue.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 14.0+tvOS 15.0+visionOS 1.0+

``` source
enum Item
```

## Topics

### Operators

static func == (MusicPlayer.Queue.Entry.Item, MusicPlayer.Queue.Entry.Item) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case musicVideo(MusicVideo)

An item that corresponds to a music video.

case song(Song)

An item that corresponds to a song.

### Instance Properties

var hashValue: Int

The hash value.

var id: MusicItemID

The unique identifier for the music player item.

var playParameters: PlayParameters?

The parameters to use to play the item.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Type Aliases

typealias ID

A type representing the stable identity of the entity associated with an instance.

### Default Implementations

CustomDebugStringConvertible Implementations

CustomStringConvertible Implementations

Decodable Implementations

Encodable Implementations

Equatable Implementations

MusicItem Implementations

## Relationships

### Conforms To

- Copyable
- CustomDebugStringConvertible
- CustomStringConvertible
- Decodable
- Encodable
- Equatable
- Hashable
- Identifiable
- MusicItem
- MusicPropertyContainer
- PlayableMusicItem
- Sendable

