

- Media Player
- MPMediaPlaylist
-  descriptionText 

Instance Property

# descriptionText

User supplied text that describes the playlist.

iOS 9.3+iPadOS 9.3+Mac Catalyst 13.1+visionOS 1.0+

``` source
var descriptionText: String? { get }
```

## See Also

### Retrieving information about a playlist

var authorDisplayName: String?

The display name for the playlist defined in the app.

var name: String?

The name of the playlist.

var persistentID: MPMediaEntityPersistentID

The persistent identifier for the playlist.

var cloudGlobalID: String?

The cloud identifier for the playlist.

var playlistAttributes: MPMediaPlaylistAttribute

The attributes associated with the playlist.

struct MPMediaPlaylistAttribute

Attributes define the type of playlist.

var seedItems: [MPMediaItem]?

The items seeded to generate the playlist; applies only to Genius playlists.

