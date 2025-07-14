

- Media Player
- MPMediaPlaylist
-  playlistAttributes 

Instance Property

# playlistAttributes

The attributes associated with the playlist.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
var playlistAttributes: MPMediaPlaylistAttribute { get }
```

## See Also

### Retrieving information about a playlist

var authorDisplayName: String?

The display name for the playlist defined in the app.

var descriptionText: String?

User supplied text that describes the playlist.

var name: String?

The name of the playlist.

var persistentID: MPMediaEntityPersistentID

The persistent identifier for the playlist.

var cloudGlobalID: String?

The cloud identifier for the playlist.

struct MPMediaPlaylistAttribute

Attributes define the type of playlist.

var seedItems: [MPMediaItem]?

The items seeded to generate the playlist; applies only to Genius playlists.

