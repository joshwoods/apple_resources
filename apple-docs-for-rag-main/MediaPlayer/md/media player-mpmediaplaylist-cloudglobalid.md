

- Media Player
- MPMediaPlaylist
-  cloudGlobalID 

Instance Property

# cloudGlobalID

The cloud identifier for the playlist.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
var cloudGlobalID: String? { get }
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

var playlistAttributes: MPMediaPlaylistAttribute

The attributes associated with the playlist.

struct MPMediaPlaylistAttribute

Attributes define the type of playlist.

var seedItems: [MPMediaItem]?

The items seeded to generate the playlist; applies only to Genius playlists.

