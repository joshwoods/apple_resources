

- MusicKit
-  MusicCatalogChartsResponse 

Structure

# MusicCatalogChartsResponse

An object that contains results for a catalog charts request.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct MusicCatalogChartsResponse
```

## Topics

### Operators

static func == (MusicCatalogChartsResponse, MusicCatalogChartsResponse) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

let albumCharts: [MusicCatalogChart&lt;Album>]

A collection of charts that contain albums.

var hashValue: Int

The hash value.

let musicVideoCharts: [MusicCatalogChart&lt;MusicVideo>]

A collection of charts that contain music videos.

let playlistCharts: [MusicCatalogChart&lt;Playlist>]

A collection of charts that contain playlists.

let songCharts: [MusicCatalogChart&lt;Song>]

A collection of charts that contain songs.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

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
- Sendable

