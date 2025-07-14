

- MusicKit
-  RecentlyPlayedMusicItem 

Enumeration

# RecentlyPlayedMusicItem

An item that represents an album, a playlist, or a station that the user has recently played.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
enum RecentlyPlayedMusicItem
```

## Topics

### Operators

static func == (RecentlyPlayedMusicItem, RecentlyPlayedMusicItem) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case album(Album)

An item that corresponds to an album.

case playlist(Playlist)

An item that corresponds to a playlist.

case station(Station)

An item that corresponds to a station.

### Instance Properties

var artwork: Artwork?

The artwork of this item.

var hashValue: Int

The hash value.

var id: MusicItemID

The unique identifier of this item.

var playParameters: PlayParameters?

The parameters to use to play this item.

var subtitle: String?

The subtitle of this item.

var title: String

The title of this item.

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
- MusicRecentlyPlayedRequestable
- PlayableMusicItem
- Sendable

