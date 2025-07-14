

- MusicKit
-  MusicLibraryRequestable 

Protocol

# MusicLibraryRequestable

A protocol for music items that your app can fetch by using a library request.

iOS 16.0+iPadOS 16.0+Mac Catalyst 17.0+macOS 14.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
protocol MusicLibraryRequestable : MusicItem
```

## Topics

### Associated Types

associatedtype LibraryFilter

The associated type that contains the set of music item properties your app uses as a filter for a library request.

**Required**

associatedtype LibrarySortProperties

The associated type that contains the set of properties your app uses to sort results for a library request.

**Required**

## Relationships

### Inherits From

- MusicItem
- Sendable

### Conforming Types

- Album
- Artist
- Genre
- MusicVideo
- Playlist
- Playlist.Entry
- Song
- Track

