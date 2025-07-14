

- MusicKit
-  MusicCatalogSearchResponse 

Structure

# MusicCatalogSearchResponse

An object that contains results for a catalog search request.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct MusicCatalogSearchResponse
```

## Topics

### Operators

static func == (MusicCatalogSearchResponse, MusicCatalogSearchResponse) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

let albums: MusicItemCollection&lt;Album>

A collection of albums.

let artists: MusicItemCollection&lt;Artist>

A collection of artists.

let curators: MusicItemCollection&lt;Curator>

A collection of curators.

var hashValue: Int

The hash value.

let musicVideos: MusicItemCollection&lt;MusicVideo>

A collection of music videos.

let playlists: MusicItemCollection&lt;Playlist>

A collection of playlists.

let radioShows: MusicItemCollection&lt;RadioShow>

A collection of radio shows.

let recordLabels: MusicItemCollection&lt;RecordLabel>

A collection of record labels.

let songs: MusicItemCollection&lt;Song>

A collection of songs.

let stations: MusicItemCollection&lt;Station>

A collection of stations.

let topResults: MusicItemCollection&lt;MusicCatalogSearchResponse.TopResult>

A collection of top results.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Enumerations

enum TopResult

An item that represents one of the top results in a catalog search response.

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

## See Also

### Catalog Search

struct MusicCatalogSearchRequest

A request that your app uses to fetch items from the Apple Music catalog using a search term.

protocol MusicCatalogSearchable

A protocol for music items that your app can fetch by using a catalog search request.

