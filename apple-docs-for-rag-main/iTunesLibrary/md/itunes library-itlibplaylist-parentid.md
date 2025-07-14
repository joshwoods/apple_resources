

- iTunes Library
- ITLibPlaylist
-  parentID 

Instance Property

# parentID

The unique persistent identifier of the playlist’s parent playlist.

Mac Catalyst 14.0+macOS 10.13+

``` source
var parentID: NSNumber? { get }
```

## Discussion

If the playlist doesn’t have a parent, this property is `nil`.

## See Also

### Getting Playlist Info

var name: String

The name or title of the playlist.

var items: [ITLibMediaItem]

The media items (tracks) in the playlist.

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

