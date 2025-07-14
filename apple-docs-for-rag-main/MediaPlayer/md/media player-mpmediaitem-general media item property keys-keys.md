

- Media Player
- MPMediaItem
-  General media item property keys 

API Collection

# General media item property keys

System-defined properties for obtaining the metadata for a media item.

## Overview

Obtain metadata for a media item by calling the value(forProperty:) method with these property keys. You can use the filterable property keys to build media property predicates, which MPMediaPropertyPredicate describes.

## Topics

### Property keys

let MPMediaItemPropertyPlaybackDuration: String

The playback duration of the media item.

let MPMediaItemPropertyAlbumTrackNumber: String

The track number of the media item, for a media item that is part of an album.

let MPMediaItemPropertyAlbumTrackCount: String

The number of tracks for the album that contains the media item.

let MPMediaItemPropertyDiscNumber: String

The disc number of the media item, for a media item that is part of a multidisc album.

let MPMediaItemPropertyDiscCount: String

The number of discs for the album that contains the media item.

let MPMediaItemPropertyArtwork: String

The artwork image for the media item.

let MPMediaItemPropertyLyrics: String

The lyrics for the media item.

let MPMediaItemPropertyReleaseDate: String

The date of the media item’s first public release.

let MPMediaItemPropertyBeatsPerMinute: String

The number of musical beats per minute for the media item.

let MPMediaItemPropertyComments: String

Textual information about the media item.

let MPMediaItemPropertyAssetURL: String

A URL that points to the media item.

let MPMediaItemPropertyIsExplicit: String

A Boolean value that indicates whether the media item contains explicit (adult) lyrics or language.

let MPMediaItemPropertyIsPreorder: String

A Boolean value that indicates whether the media item is a preorder.

let MPMediaItemPropertyPlaybackStoreID: String

The identifier for enqueueing store tracks.

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

let MPMediaItemPropertyIsCompilation: String

A Boolean value that indicates whether the media item is part of a compilation.

let MPMediaItemPropertyIsCloudItem: String

A Boolean value that indicates whether the media item is an iCloud item.

let MPMediaItemPropertyMediaType: String

The media type of the media item.

let MPMediaItemPropertyPersistentID: String

The key for the persistent identifier for the media item.

let MPMediaItemPropertyPlayCount: String

The number of times the user plays the media item.

let MPMediaItemPropertyPodcastPersistentID: String

The persistent identifier for an audio podcast.

let MPMediaItemPropertyPodcastTitle: String

The title of a podcast.

let MPMediaItemPropertyTitle: String

The title or name of the media item.

## See Also

### Media item types and keys

struct MPMediaType

The properties for defining the type for a media item.

User-defined property keys

Properties for obtaining user-defined metadata for a media item.

