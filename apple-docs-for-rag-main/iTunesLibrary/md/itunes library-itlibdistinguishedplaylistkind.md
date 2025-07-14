

- iTunes Library
-  ITLibDistinguishedPlaylistKind 

Enumeration

# ITLibDistinguishedPlaylistKind

These constants specify the possible kinds of distinguished playlists.

Mac Catalyst 14.0+macOS 10.13+

``` source
enum ITLibDistinguishedPlaylistKind
```

## Topics

### Distinguished Playlist Kinds

case kindNone

The playlist isn’t a distinguished playlist.

case kindMovies

The playlist contains all the movies in the iTunes library.

case kindTVShows

The playlist contains all the TV shows in the iTunes library.

case kindMusic

The playlist contains all the music items in the iTunes library.

case kindAudiobooks

The playlist contains all the audiobooks in the iTunes library.

static var kindBooks: ITLibDistinguishedPlaylistKind

The playlist contains all the audiobooks in the iTunes library.

case kindRingtones

The playlist contains all the iOS ringtones in the iTunes library.

case kindPodcasts

The playlist contains all the podcasts in the iTunes library.

case kindVoiceMemos

The playlist contains all the voice memos in the iTunes library.

case kindPurchases

The playlist contains all the user’s purchases from the iTunes Store.

case kindiTunesU

The playlist contains all the user’s iTunes U items.

case kind90sMusic

The default Smart Playlist that iTunes creates of the user’s music from the 1990s.

case kindMyTopRated

The default Smart Playlist that iTunes creates of the user’s top rated media items.

case kindTop25MostPlayed

The default Smart Playlist that iTunes creates of the user’s 25 most played media items.

case kindRecentlyPlayed

The default Smart Playlist that iTunes creates of the user’s most recently played media items.

case kindRecentlyAdded

The default Smart Playlist that iTunes creates of the user’s most recently added media items.

case kindMusicVideos

The default Smart Playlist that iTunes creates of the user’s music videos.

case kindClassicalMusic

The default Smart Playlist that iTunes creates of the user’s classical music.

case kindLibraryMusicVideos

The playlist contains all the music videos in the iTunes library.

case kindHomeVideos

The playlist contains all the user’s home videos in the iTunes library.

case kindApplications

The playlist contains all the user’s iOS apps in the iTunes library.

case kindLovedSongs

The playlist contains all the user’s loved music.

case kindMusicShowsAndMovies

The default Smart Playlist that iTunes creates of the user’s music shows and movies.

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

### Getting Playlist Info

var name: String

The name or title of the playlist.

var items: [ITLibMediaItem]

The media items (tracks) in the playlist.

var parentID: NSNumber?

The unique persistent identifier of the playlist’s parent playlist.

var isPrimary: Bool

A Boolean value that indicates whether the playlist is the primary playlist.

var isVisible: Bool

A Boolean value that indicates whether the playlist is visible to the user in iTunes.

var distinguishedKind: ITLibDistinguishedPlaylistKind

An indication of whether the playlist has a special distinction.

var kind: ITLibPlaylistKind

An indication of the type of playlist.

enum ITLibPlaylistKind

These constants specify the possible kinds of playlists.

