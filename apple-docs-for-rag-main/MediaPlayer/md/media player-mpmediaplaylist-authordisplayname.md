

- Media Player
- MPMediaPlaylist
-  authorDisplayName 

Instance Property

# authorDisplayName

The display name for the playlist defined in the app.

iOS 9.3+iPadOS 9.3+Mac Catalyst 13.1+visionOS 1.0+

``` source
var authorDisplayName: String? { get }
```

## Discussion

The system requires this property for 3rd party apps. Defaults to the app display name when not defined.

## See Also

### Retrieving information about a playlist

var descriptionText: String?

User supplied text that describes the playlist.

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

