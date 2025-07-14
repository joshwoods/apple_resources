

- iTunes Library
-  ITLibPlaylist 

Class

# ITLibPlaylist

This class describes a playlist in the iTunes library.

Mac Catalyst 14.0+macOS 10.13+

``` source
class ITLibPlaylist
```

## Overview

A *playlist* is a collection of media items (tracks). The user creates and organizes playlists manually, or iTunes automatically generates them. Playlists are media entities. Each contains a unique identifier and a set of properties. Playlists can form a hierarchical structure. In those cases, the parentID property of ITLibPlaylist returns the persistent ID of the parent playlist.

## Topics

### Getting Playlist Info

var name: String

The name or title of the playlist.

var items: [ITLibMediaItem]

The media items (tracks) in the playlist.

var parentID: NSNumber?

The unique persistent identifier of the playlist’s parent playlist.

var isPrimary: Bool

A Boolean value that indicates whether the playlist is the primary playlist.

var isVisible: Bool

A Boolean value that indicates whether the playlist is visible to the user in iTunes.

var distinguishedKind: ITLibDistinguishedPlaylistKind

An indication of whether the playlist has a special distinction.

var kind: ITLibPlaylistKind

An indication of the type of playlist.

enum ITLibPlaylistKind

These constants specify the possible kinds of playlists.

enum ITLibDistinguishedPlaylistKind

These constants specify the possible kinds of distinguished playlists.

### Playlist Properties

let ITLibPlaylistPropertyAllItemsPlaylist: String

A Boolean value that indicates whether the API exposes every item in the playlist.

let ITLibPlaylistPropertyDistinguisedKind: String

An indication of whether the playlist has a special distinction.

let ITLibPlaylistPropertyItems: String

The media items (tracks) in the playlist.

let ITLibPlaylistPropertyKind: String

An indication of the type of playlist.

let ITLibPlaylistPropertyPrimary: String

A Boolean value that indicates whether the playlist is the primary playlist.

let ITLibPlaylistPropertyName: String

The name or title of the playlist.

let ITLibPlaylistPropertyParentPersistentID: String

The unique persistent identifier of the playlist’s parent playlist.

let ITLibPlaylistPropertyVisible: String

A Boolean value that indicates whether the playlist is visible to the user in iTunes.

### Deprecated

var isAllItemsPlaylist: Bool

Indicates whether the API exposes every item in the playlist.

Deprecated

var isMaster: Bool

A Boolean value that indicates whether the playlist represents the entire iTunes library.

Deprecated

let ITLibPlaylistPropertyMaster: String

A Boolean value that indicates whether the playlist represents the entire iTunes library.

Deprecated

## Relationships

### Inherits From

- ITLibMediaEntity

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Albums and Playlists

class ITLibAlbum

This class provides information about an album in the iTunes library.

