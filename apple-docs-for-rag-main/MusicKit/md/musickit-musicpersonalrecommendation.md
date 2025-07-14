

- MusicKit
-  MusicPersonalRecommendation 

Structure

# MusicPersonalRecommendation

An object that contains recommended items based on the user’s library and listening history.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct MusicPersonalRecommendation
```

## Topics

### Operators

static func == (MusicPersonalRecommendation, MusicPersonalRecommendation) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

var albums: MusicItemCollection&lt;Album>

The albums for the personal recommendation.

var hashValue: Int

The hash value.

let id: MusicItemID

The unique identifier for the personal recommendation.

var items: MusicItemCollection&lt;MusicPersonalRecommendation.Item>

The items for the personal recommendation.

let nextRefreshDate: Date?

The next date for refreshing the personal recommendation.

var playlists: MusicItemCollection&lt;Playlist>

The playlists for the personal recommendation.

let reason: String?

The reason for the personal recommendation.

var stations: MusicItemCollection&lt;Station>

The stations for the personal recommendation.

let title: String?

The title for the personal recommendation.

var types: [any MusicPersonalRecommendationItem.Type]

The types of items in the personal recommendation.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Type Aliases

typealias ID

A type representing the stable identity of the entity associated with an instance.

### Enumerations

enum Item

An item that represents an album, a playlist, or a station for a personal recommendation.

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
- Sendable

