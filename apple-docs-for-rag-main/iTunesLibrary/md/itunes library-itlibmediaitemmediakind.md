

- iTunes Library
-  ITLibMediaItemMediaKind 

Enumeration

# ITLibMediaItemMediaKind

These constants specify the possible media kinds of a media item.

Mac Catalyst 14.0+macOS 10.13+

``` source
enum ITLibMediaItemMediaKind
```

## Topics

### Media Kinds

case kindUnknown

The media item kind is unknown.

case kindSong

The media item is a song.

case kindMovie

The media item is a movie.

case kindPodcast

The media item is an audio or a video podcast.

case kindAudiobook

The media item is an audiobook.

case kindPDFBooklet

The media item is an unwrapped PDF file that’s part of a music album.

case kindMusicVideo

The media item is a music video.

case kindTVShow

The media item is a TV show.

case kindInteractiveBooklet

The media item is a QuickTime movie with embedded Flash.

Deprecated

case kindHomeVideo

The media item is a non-iTunes Store movie.

case kindRingtone

The media item is an iOS ringtone.

case kindDigitalBooklet

The media item is an iTunes Extra or an iTunes LP item.

case kindIOSApplication

The media item is an iOS app.

case kindVoiceMemo

The media item is a recorded voice memo.

case kindiTunesU

The media item is an iTunes U audio or video file.

case kindBook

The media item is an EPUB file or an iBooks Author book.

case kindPDFBook

The media item is a PDF file that iTunes treats as a book unless the user overrides it.

case kindAlertTone

The media item is an audio tone that’s not a protected ringtone on an iOS device.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

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

