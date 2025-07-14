

- iTunes Library
-  ITLibMediaItem 

Class

# ITLibMediaItem

This class describes a media item (a track) in the iTunes library, such as a song, a video, or a podcast.

Mac Catalyst 14.0+macOS 10.13+

``` source
class ITLibMediaItem
```

## Overview

Like all media entities, each media item has a unique identifier and a set of properties.

## Topics

### Getting Media Item Info

var title: String

The title of the media item.

var sortTitle: String?

The title of the media item to use when sorting.

var artist: ITLibArtist?

Information about the artist that iTunes associates with the media item.

var composer: String

The name of the composer that iTunes associates with the media item.

var sortComposer: String?

The name to use when sorting by composer.

var rating: Int

The rating of the media item.

var isRatingComputed: Bool

A Boolean value that indicates whether iTunes computes the media item’s rating from its album rating.

var startTime: Int

If nonzero, the actual time playback of the media item starts instead of 0:00 (in milliseconds).

var stopTime: Int

If nonzero, the actual time playback of the media item stops versus the total time (in milliseconds).

var album: ITLibAlbum

The album of the media item.

var genre: String

The genre of the media item, if any.

var kind: String?

The kind of media item file, such as an MPEG audio file.

var mediaKind: ITLibMediaItemMediaKind

The kind of media item.

var totalTime: Int

The length of the media item in milliseconds.

var trackNumber: Int

The position of the media item within its album.

var category: String?

The podcast category of the media item, if the media item is a podcast.

var description: String?

The description of the media item, if it’s a podcast.

var contentRating: String?

The content rating of the media item.

var lyricsContentRating: ITLibMediaItemLyricsContentRating

The content rating of the media item’s lyrics.

var addedDate: Date?

The date and time that the user added the media item to the iTunes library.

var modifiedDate: Date?

The date and time that iTunes last modified the media item.

var bitrate: Int

The bitrate of the media item in kbit/s.

var sampleRate: Int

The sample rate of the media item in samples-per-second.

var beatsPerMinute: Int

The beats-per-minute (BPM) of the media item.

var playCount: Int

The number of times the user has played the media item.

var lastPlayedDate: Date?

The date and time the user last played the media item, or `nil` if the user hasn’t played it.

var location: URL?

The location of the media item on disk.

var locationType: ITLibMediaItemLocationType

The type of the media item with respect to its location.

var hasArtworkAvailable: Bool

A Boolean value that indicates whether the media item has artwork.

var artwork: ITLibArtwork?

The artwork of the media item.

var comments: String?

Any comments that iTunes associates with the media item.

var isPurchased: Bool

A Boolean value that indicates whether the user purchased the media item from the iTunes Store.

var isDRMProtected: Bool

A Boolean value that indicates whether the media item has digital rights management (DRM) protection.

var isVideo: Bool

A Boolean value that indicates whether this media item is a video, such as a TV show, video podcast, or movie.

var videoInfo: ITLibMediaItemVideoInfo?

Video information (such as width and height) about the media item, if it’s a video.

var releaseDate: Date?

The release date of the media item.

var year: Int

The release year of the media item.

var skipCount: Int

The number of times that the user skipped the media item.

var skipDate: Date?

The date and time that the user last skipped the media item.

var voiceOverLanguage: String?

The voice-over language of the media item.

Deprecated

var volumeAdjustment: Int

The volume adjustment for the media item, if any.

var volumeNormalizationEnergy: Int

The volume normalization energy that iTunes applies to the media item to bring the average or peak amplitude to a target level.

var isUserDisabled: Bool

A Boolean value that indicates whether the user disabled the media item.

var grouping: String?

The grouping of the media item that the user specifies or that iTunes specifies in the file’s metadata.

var fileSize: UInt64

The size in bytes of this media item on disk.

var isCloud: Bool

A Boolean value that indicates whether this media item is an iTunes Match or an iTunes in the Cloud item.

var playStatus: ITLibMediaItemPlayStatus

The play status for the media.

enum ITLibMediaItemMediaKind

These constants specify the possible media kinds of a media item.

enum ITLibMediaItemLocationType

These constants specify the location type of a media item.

enum ITLibMediaItemLyricsContentRating

These constants specify the possible ratings of media item lyrics.

enum ITLibMediaItemPlayStatus

These constants specify the play status of the media item.

### Media Item Properties

let ITLibMediaEntityPropertyPersistentID: String

The unique identifier of the media entity.

let ITLibMediaItemPropertyAddedDate: String

The date and time the user added the media item to the iTunes library.

let ITLibMediaItemPropertyAlbumArtist: String

The name of the artist that iTunes associates with the media item’s album.

let ITLibMediaItemPropertyAlbumDiscCount: String

The number of discs in the media item’s album.

let ITLibMediaItemPropertyAlbumDiscNumber: String

The disc number in the media item’s album.

let ITLibMediaItemPropertyAlbumIsCompilation: String

This property indicates whether the album of the media item is a compilation.

let ITLibMediaItemPropertyAlbumIsGapless: String

This property indicates whether the media item’s album is gapless.

let ITLibMediaItemPropertyAlbumRating: String

The rating of the media item’s album.

let ITLibMediaItemPropertyAlbumRatingComputed: String

This property indicates whether iTunes computes the rating of the media item’s album from the ratings of individual tracks in the album.

let ITLibMediaItemPropertyAlbumTitle: String

The title of the media item’s album.

let ITLibMediaItemPropertyAlbumTrackCount: String

The track count of the media item’s album.

let ITLibMediaItemPropertyArtistName: String

The name of the artist that iTunes associates with the media item.

let ITLibMediaItemPropertyArtwork: String

The artwork for the media item.

let ITLibMediaItemPropertyBeatsPerMinute: String

The beats-per-minute (BPM) of the media item.

let ITLibMediaItemPropertyBitRate: String

The bitrate of the media item in kbit/s.

let ITLibMediaItemPropertyCategory: String

The podcast category of the media item, if the media item is a podcast.

let ITLibMediaItemPropertyComments: String

Any comments that iTunes associates with the media item.

let ITLibMediaItemPropertyComposer: String

The name of the composer that iTunes associates with the media item.

let ITLibMediaItemPropertyContentRating: String

The extended content rating of the media item.

let ITLibMediaItemPropertyDescription: String

A podcast description of the media item, if the media item is a podcast.

let ITLibMediaItemPropertyFileSize: String

The size in bytes of the media item on disk.

let ITLibMediaItemPropertyGenre: String

The genre that iTunes associates with the media item.

let ITLibMediaItemPropertyGrouping: String

The grouping of the media item.

let ITLibMediaItemPropertyHasArtwork: String

This property indicates whether the media item has artwork.

let ITLibMediaItemPropertyIsDRMProtected: String

This property indicates whether the media item has digital rights management (DRM) protection.

let ITLibMediaItemPropertyIsPurchased: String

This property indicates whether the media item is a purchased media item.

let ITLibMediaItemPropertyIsUserDisabled: String

This property indicates whether the user disabled the media item.

let ITLibMediaItemPropertyIsVideo: String

This property indicates whether the media item is a video media item, such as a video podcast or movie.

let ITLibMediaItemPropertyKind: String

The kind of media item file, such as an MPEG audio file.

let ITLibMediaItemPropertyLastPlayDate: String

The date and time the user last played the media item in iTunes, or `nil` if the user hasn’t played the media item.

let ITLibMediaItemPropertyLocation: String

The location of the media item on disk.

let ITLibMediaItemPropertyLocationType: String

The type of the media item with respect to its location.

let ITLibMediaItemPropertyLyricsContentRating: String

The content rating of the media item’s lyrics.

let ITLibMediaItemPropertyMediaKind: String

The media kind of the media item.

let ITLibMediaItemPropertyModifiedDate: String

The date and time that iTunes last modified the media item.

let ITLibMediaItemPropertyMovementCount: String

let ITLibMediaItemPropertyMovementName: String

let ITLibMediaItemPropertyMovementNumber: String

let ITLibMediaItemPropertyPlayCount: String

The number of times the user has played the media item in iTunes.

let ITLibMediaItemPropertyPlayStatus: String

The play status of the media item.

let ITLibMediaItemPropertyRating: String

The rating of the media item.

let ITLibMediaItemPropertyRatingComputed: String

This property indicates whether iTunes computes the media item’s rating.

let ITLibMediaItemPropertyReleaseDate: String

The release date of the media item.

let ITLibMediaItemPropertySampleRate: String

The sample rate of the media item in samples-per-second.

let ITLibMediaItemPropertySize: String

The size in bytes of the media item on disk.

Deprecated

let ITLibMediaItemPropertySkipDate: String

The date and time that the user last skipped the media item.

let ITLibMediaItemPropertySortAlbumArtist: String

The name of the artist that iTunes associates with the media item’s album, for use when sorting.

let ITLibMediaItemPropertySortAlbumTitle: String

The title of the media item’s album, for use when sorting.

let ITLibMediaItemPropertySortArtistName: String

The name of the media item’s artist, for use when sorting.

let ITLibMediaItemPropertySortComposer: String

The name of the composer that iTunes associates with the media item, for use when sorting.

let ITLibMediaItemPropertySortTitle: String

The title of the media item to use when sorting.

let ITLibMediaItemPropertyStartTime: String

If nonzero, the actual time that playback for the media item starts instead of 0:00 (in milliseconds).

let ITLibMediaItemPropertyStopTime: String

If nonzero, the actual time that playback for the media item stops versus the total time (in milliseconds).

let ITLibMediaItemPropertyTitle: String

The title of the media item.

let ITLibMediaItemPropertyTotalTime: String

The length of the media item in milliseconds.

let ITLibMediaItemPropertyTrackNumber: String

The numerical position of the media item within its album.

let ITLibMediaItemPropertyUserSkipCount: String

The number of times that the user skipped the media item.

let ITLibMediaItemPropertyVideoEpisode: String

The name of the episode, if the media item is an episode of a TV series.

let ITLibMediaItemPropertyVideoEpisodeOrder: String

The order of the episode, if the media item is an episode of a TV series.

let ITLibMediaItemPropertyVideoHeight: String

The height in pixels, if the media item is a video.

let ITLibMediaItemPropertyVideoIsHD: String

This property indicates whether a video media item is high-definition.

let ITLibMediaItemPropertyVideoSeason: String

The corresponding TV season, if the media item is an episode of a TV series.

let ITLibMediaItemPropertyVideoSeries: String

The name of the corresponding TV series, if the media item is an episode in a TV series.

let ITLibMediaItemPropertyVideoSortSeries: String

The sorting name of the corresponding TV series, if the media item is an episode in a TV series.

let ITLibMediaItemPropertyVideoWidth: String

The width in pixels, if the media item is a video.

let ITLibMediaItemPropertyVoiceOverLanguage: String

The voice-over language of the media item.

Deprecated

let ITLibMediaItemPropertyVolumeAdjustment: String

The volume adjustment for the media item, if any.

let ITLibMediaItemPropertyVolumeNormalizationEnergy: String

The volume normalization energy that iTunes applies to the media item to bring the average or peak amplitude to a target level.

let ITLibMediaItemPropertyWork: String

let ITLibMediaItemPropertyYear: String

The release year of the media item.

### Deprecated

var fileType: Int

The file type of the media item.

Deprecated

var size: Int

The size in bytes of the media item on disk.

Deprecated

let ITLibMediaItemPropertyFileType: String

The file type of the media item.

Deprecated

## Relationships

### Inherits From

- ITLibMediaEntity

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Media Items

class ITLibMediaEntity

This class describes a media entity, which can be a media item, such as an audio track.

class ITLibArtist

This class represents an artist, such as the performer of a song.

class ITLibArtwork

This class represents the artwork for a media item.

class ITLibMediaItemVideoInfo

This class encapsulates the video information of a video media item.

