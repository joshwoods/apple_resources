

- MusicKit
-  MusicLibrarySearchResponse 

Structure

# MusicLibrarySearchResponse

An object that contains results for a library search request.

iOS 16.0+iPadOS 16.0+Mac Catalyst 17.0+macOS 14.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct MusicLibrarySearchResponse
```

## Topics

### Operators

static func == (MusicLibrarySearchResponse, MusicLibrarySearchResponse) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

let albums: MusicItemCollection&lt;Album>

A collection of albums.

let artists: MusicItemCollection&lt;Artist>

A collection of artists.

var hashValue: Int

The hash value.

let musicVideos: MusicItemCollection&lt;MusicVideo>

A collection of music videos.

let playlists: MusicItemCollection&lt;Playlist>

A collection of playlists.

let songs: MusicItemCollection&lt;Song>

A collection of songs.

let topResults: MusicItemCollection&lt;MusicLibrarySearchResponse.TopResult>

A collection of top results.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Enumerations

enum TopResult

An item that represents one of the top results in a library search response.

### Default Implementations

CustomDebugStringConvertible Implementations

CustomStringConvertible Implementations

Equatable Implementations

## Relationships

### Conforms To

- Copyable
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- Sendable

