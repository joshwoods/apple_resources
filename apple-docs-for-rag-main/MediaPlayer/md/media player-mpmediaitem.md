

- Media Player
-  MPMediaItem 

Class

# MPMediaItem

A collection of properties that represents a single item in the media library.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+tvOS 14.0+visionOS 1.0+

``` source
class MPMediaItem
```

## Overview

A media item has an overall unique identifier, accessed using the MPMediaItemPropertyPersistentID property key, as well as specific identifiers for its metadata. These identifiers persists across application launches.

A media item can have a wide range of metadata associated with it. You access this metadata using the value(forProperty:) method along with the property keys described in this document. You can also access metadata in a batch fashion using the enumerateValues(forProperties:using:) method. Anytime the app accesses more than one property, enumerating over a set of property keys is more efficient than fetching each individual property. MPMediaEntity defines both of these methods, the abstract superclass of MPMediaItemCollection, and described in `MPMediaEntity`.

You use attributes of media items to build media queries for searching the Media library. MPMediaType, General media item property keys, and `Podcast Item Property Keys` describe these attributes. In addition, Media entity property keys describes the MPMediaEntityPropertyPersistentID property, and MPMediaQuery describes media queries.

## Topics

### Media item properties

var albumArtist: String?

The primary performing artist for an album.

var albumArtistPersistentID: MPMediaEntityPersistentID

The persistent identifier for the primary performing artist for an album.

var albumPersistentID: MPMediaEntityPersistentID

The persistent identifier for an album.

var albumTitle: String?

The title of an album, such as *Live on Mars*, rather than the title of an individual song on the album, such as “Crater Dance.”

var albumTrackCount: Int

The number of tracks for the album that contains the media item.

var albumTrackNumber: Int

The track number of the media item, for a media item that’s part of an album.

var artist: String?

The performing artists for a media item, which may vary from the primary artist for the album that a media item belongs to.

var artistPersistentID: MPMediaEntityPersistentID

The persistent identifier for an artist.

var artwork: MPMediaItemArtwork?

The artwork image for the media item.

var assetURL: URL?

The URL that points to the media item.

var beatsPerMinute: Int

The number of musical beats per minute for the media item.

var bookmarkTime: TimeInterval

The time of the user’s most recent interaction with the bookmark in the media item.

var isCloudItem: Bool

A Boolean value that indicates whether the media item is an iCloud Music Library item.

var comments: String?

Textual information about the media item.

var isCompilation: Bool

A Boolean value that indicates whether the media item is part of a compilation.

var isPreorder: Bool

A Boolean value that indicates whether the media item is a preorder.

var composer: String?

The musical composer for the media item.

var composerPersistentID: MPMediaEntityPersistentID

The persistent identifier for a composer.

var dateAdded: Date

The date the user adds the media item to the library.

var discCount: Int

The number of discs for the album that contains the media item.

var discNumber: Int

The disc number of the media item, for a media item that’s part of a multidisc album.

var isExplicitItem: Bool

A Boolean value that indicates whether the media item has explicit (adult) lyrics or language.

var genre: String?

The music or film genre of the media item.

var genrePersistentID: MPMediaEntityPersistentID

The persistent identifier for a genre.

var lastPlayedDate: Date?

The most recent play date of the media item.

var lyrics: String?

The lyrics for the media item.

var mediaType: MPMediaType

The media type of the media item.

var persistentID: MPMediaEntityPersistentID

The persistent identifier for the media item.

var playCount: Int

The number of times the user plays the media item.

var playbackDuration: TimeInterval

The playback duration of the media item.

var playbackStoreID: String

The ID of a media item from the Apple Music catalog.

var podcastPersistentID: MPMediaEntityPersistentID

The persistent identifier for an audio podcast.

var podcastTitle: String?

The title of a podcast, such as *This Martian Drudgery*, rather than the title of an individual episode of a podcast, such as “Episode 12: Another Cold Day at the Pole.”

var hasProtectedAsset: Bool

A Boolean value that indicates whether the media item has a protected asset.

var rating: Int

The user-specified rating of the media item.

var releaseDate: Date?

The date of the media item’s first public release.

var skipCount: Int

The number of times the user skips playing the media item.

var title: String?

The title or name of the media item.

var userGrouping: String?

Grouping information for the media item.

### Obtaining group properties

class func persistentIDProperty(forGroupingType: MPMediaGrouping) -> String

Obtains the persistent identifier key for a specified grouping type.

class func titleProperty(forGroupingType: MPMediaGrouping) -> String

Obtains the title key for a specified grouping type.

### Media item types and keys

struct MPMediaType

The properties for defining the type for a media item.

General media item property keys

System-defined properties for obtaining the metadata for a media item.

User-defined property keys

Properties for obtaining user-defined metadata for a media item.

## Relationships

### Inherits From

- MPMediaEntity

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding

## See Also

### Media items and playlists

class MPMediaItemArtwork

A graphical image, such as music album cover art, associated with a media item.

class MPMediaItemCollection

A sorted set of media items from the media library.

class MPMediaPlaylist

A playable collection of related media items.

class MPMediaPlaylistCreationMetadata

A set of attributes for describing a playlist when creating it.

class MPMediaEntity

The abstract superclass for media items, media item collections, and media playlist instances.

