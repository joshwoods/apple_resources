

- MusicKit
-  Station 

Structure

# Station

A music item that represents a station.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct Station
```

## Topics

### Operators

static func == (Station, Station) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

var artwork: Artwork?

The station artwork.

var contentRating: ContentRating?

The rating of the content that potentially plays while playing the station.

var duration: TimeInterval?

The duration of the stream.

var editorialNotes: EditorialNotes?

The notes about the station that appear in the Music app.

var episodeNumber: Int?

The episode number of the station.

var hashValue: Int

The hash value.

let id: MusicItemID

The unique identifier for the station.

var isLive: Bool

A Boolean value that indicates whether the station is live.

var name: String

The name of the station.

var playParameters: PlayParameters?

The parameters to use to play the station.

var stationProviderName: String?

The name of the entity that provides the station.

var url: URL?

The URL for the station.

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

FilterableMusicItem Implementations

MusicItem Implementations

## Relationships

### Conforms To

- Copyable
- CustomDebugStringConvertible
- CustomStringConvertible
- Decodable
- Encodable
- Equatable
- FilterableMusicItem
- Hashable
- Identifiable
- MusicCatalogSearchable
- MusicItem
- MusicPersonalRecommendationItem
- MusicPropertyContainer
- MusicRecentlyPlayedRequestable
- PlayableMusicItem
- Sendable

## See Also

### Music Items

struct Album

A music item that represents an album.

struct Artist

A music item that represents an artist.

struct Curator

A music item that represents a curator.

struct Genre

A music item that represents a genre.

struct MusicVideo

A music item that represents a music video.

struct Playlist

A music item that represents a playlist.

struct RadioShow

A music item that represents a radio show.

struct RecordLabel

A music item that represents a record label.

struct Song

A music item that represents a song.

enum Track

A music item that represents a track.

