

- iTunes Library
- ITLibrary
-  allPlaylists 

Instance Property

# allPlaylists

All the playlists in the iTunes library.

Mac Catalyst 14.0+macOS 10.13+

``` source
var allPlaylists: [ITLibPlaylist] { get }
```

## Return Value

An array of ITLibPlaylist items.

## See Also

### Getting iTunes Library Info

var allMediaItems: [ITLibMediaItem]

All the media items (tracks) in the iTunes library.

var apiMajorVersion: Int

The major version number of the API the iTunesLibrary framework exposes.

var apiMinorVersion: Int

The minor version number of the API the iTunesLibrary framework exposes.

var applicationVersion: String

The version of iTunes that created or modified the iTunes library you’re accessing.

var mediaFolderLocation: URL?

The location of the iTunes music folder.

var shouldShowContentRating: Bool

A Boolean value indicating whether to show content rating labels.

