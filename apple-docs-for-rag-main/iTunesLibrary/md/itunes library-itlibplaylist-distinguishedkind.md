

- iTunes Library
- ITLibPlaylist
-  distinguishedKind 

Instance Property

# distinguishedKind

An indication of whether the playlist has a special distinction.

Mac Catalyst 14.0+macOS 10.13+

``` source
var distinguishedKind: ITLibDistinguishedPlaylistKind { get }
```

## Discussion

*Distinguished playlists* are special playlists that iTunes generates to organize media items inside the library. If the playlist isn’t a distinguished playlist, this property returns ITLibDistinguishedPlaylistKind.kindNone.

## See Also

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

var kind: ITLibPlaylistKind

An indication of the type of playlist.

enum ITLibPlaylistKind

These constants specify the possible kinds of playlists.

enum ITLibDistinguishedPlaylistKind

These constants specify the possible kinds of distinguished playlists.

