

- iTunes Library
-  ITLibPlaylistKind 

Enumeration

# ITLibPlaylistKind

These constants specify the possible kinds of playlists.

Mac Catalyst 14.0+macOS 10.13+

``` source
enum ITLibPlaylistKind
```

## Topics

### Playlist Kinds

case regular

A standard playlist that the user or iTunes creates, such as *Music*, *Movies*, *Pop Mix*, or *My Awesome Playlist*.

case smart

A playlist with contents that iTunes generates by evaluating a set of rules, such as *90s Music* or *Songs from 1999*.

case genius

A playlist iTunes creates of songs that go well with a song the user specifies.

case folder

A playlist folder that the user or iTunes creates, such as *My Playlist Folder* or *Genius Mixes*.

case geniusMix

An ongoing playlist in a particular genre—like a commercial-free radio station playing the user’s favorite songs—that iTunes creates from music in the user’s iTunes library.

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

enum ITLibDistinguishedPlaylistKind

These constants specify the possible kinds of distinguished playlists.

