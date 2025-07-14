

- iTunes Library
- ITLibPlaylist
-  isVisible 

Instance Property

# isVisible

A Boolean value that indicates whether the playlist is visible to the user in iTunes.

Mac Catalyst 14.0+macOS 10.13+

``` source
var isVisible: Bool { get }
```

## Discussion

There are some playlists that iTunes hides, uses, and maintains without displaying them as playlists to the user. Tracks can still be visible when they’re in a playlist that’s not visible.

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

var distinguishedKind: ITLibDistinguishedPlaylistKind

An indication of whether the playlist has a special distinction.

var kind: ITLibPlaylistKind

An indication of the type of playlist.

enum ITLibPlaylistKind

These constants specify the possible kinds of playlists.

enum ITLibDistinguishedPlaylistKind

These constants specify the possible kinds of distinguished playlists.

