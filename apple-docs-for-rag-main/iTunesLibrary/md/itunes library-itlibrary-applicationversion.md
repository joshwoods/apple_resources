

- iTunes Library
- ITLibrary
-  applicationVersion 

Instance Property

# applicationVersion

The version of iTunes that created or modified the iTunes library you’re accessing.

Mac Catalyst 14.0+macOS 10.13+

``` source
var applicationVersion: String { get }
```

## See Also

### Getting iTunes Library Info

var allMediaItems: [ITLibMediaItem]

All the media items (tracks) in the iTunes library.

var allPlaylists: [ITLibPlaylist]

All the playlists in the iTunes library.

var apiMajorVersion: Int

The major version number of the API the iTunesLibrary framework exposes.

var apiMinorVersion: Int

The minor version number of the API the iTunesLibrary framework exposes.

var mediaFolderLocation: URL?

The location of the iTunes music folder.

var shouldShowContentRating: Bool

A Boolean value indicating whether to show content rating labels.

