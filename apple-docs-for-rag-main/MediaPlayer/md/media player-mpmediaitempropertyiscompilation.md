

- Media Player
-  MPMediaItemPropertyIsCompilation 

Global Variable

# MPMediaItemPropertyIsCompilation

A Boolean value that indicates whether the media item is part of a compilation.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.12.2+tvOS 9.0+visionOS 1.0+watchOS 5.0+

``` source
let MPMediaItemPropertyIsCompilation: String
```

## Discussion

This property corresponds to the “Part of a compilation” checkbox in the Info tab of the Get Info dialog in iTunes. Its associated value is an NSNumber object representing a Boolean value.

## See Also

### Filterable property keys

let MPMediaItemPropertyAlbumArtist: String

The primary performing artist for an album.

let MPMediaItemPropertyAlbumArtistPersistentID: String

The persistent identifier for an album artist.

let MPMediaItemPropertyAlbumPersistentID: String

The key for the persistent identifier for an album.

let MPMediaItemPropertyAlbumTitle: String

The title of an album.

let MPMediaItemPropertyArtist: String

The performing artists for a media item — which may vary from the primary artist for the album that a media item belongs to.

let MPMediaItemPropertyArtistPersistentID: String

The key for the persistent identifier for an artist.

let MPMediaItemPropertyComposer: String

The musical composer for the media item.

let MPMediaItemPropertyComposerPersistentID: String

The persistent identifier for a composer.

let MPMediaItemPropertyGenre: String

The music or film genre of the media item.

let MPMediaItemPropertyGenrePersistentID: String

The persistent identifier for a genre.

let MPMediaItemPropertyHasProtectedAsset: String

A Boolean value that indicates the media item has DRM protection so it can’t play through a standard playback API.

let MPMediaItemPropertyIsCloudItem: String

A Boolean value that indicates whether the media item is an iCloud item.

let MPMediaItemPropertyMediaType: String

The media type of the media item.

let MPMediaItemPropertyPersistentID: String

The key for the persistent identifier for the media item.

let MPMediaItemPropertyPlayCount: String

The number of times the user plays the media item.

