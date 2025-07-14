

- Media Player
-  MPMediaPlaylistPropertyPlaylistAttributes 

Global Variable

# MPMediaPlaylistPropertyPlaylistAttributes

The attributes associated with the playlist.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
let MPMediaPlaylistPropertyPlaylistAttributes: String
```

## Discussion

Value is an NSNumber object containing an NSInteger data type. Fields in the `NSInteger` identify the attributes of the playlist. A playlist may have any combination of attributes described in MPMediaPlaylistAttribute. Can be used to build a media property predicate as described in MPMediaQuery.

## See Also

### Property keys

let MPMediaPlaylistPropertyAuthorDisplayName: String

App defined name for the playlist.

let MPMediaPlaylistPropertyName: String

The name of the playlist.

let MPMediaPlaylistPropertyDescriptionText: String

Descriptive text for the playlist.

let MPMediaPlaylistPropertyPersistentID: String

The persistent identifier for the playlist.

let MPMediaPlaylistPropertyCloudGlobalID: String

The cloud identifier for the playlist.

let MPMediaPlaylistPropertySeedItems: String

The items seeded to generate the playlist; applies only to Genius playlists.

