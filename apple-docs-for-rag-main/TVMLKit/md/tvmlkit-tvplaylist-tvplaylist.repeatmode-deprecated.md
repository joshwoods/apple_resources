

- TVMLKit
- TVPlaylist
-  TVPlaylist.RepeatMode Deprecated

Enumeration

# TVPlaylist.RepeatMode

The modes that indicate how or whether media items can be replayed.

tvOS 12.0–18.0Deprecated

``` source
enum RepeatMode
```

Deprecated

Please use SwiftUI or UIKit

## Topics

### Replay Modes

case all

Replay all of the media items in the playlist.

case one

Replay the currently playing media item.

case none

Replay none of the media items in the playlist.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Retrieving Playlist Information

var mediaItems: [TVMediaItem]

An array of media items contained in the playlist.

Deprecated

var userInfo: [String : Any]?

User-defined metadata, like a developer-specific identifier, for a playlist.

Deprecated

var repeatMode: TVPlaylist.RepeatMode

A mode that determines how media items are replayed.

Deprecated

var endAction: TVPlaylist.EndAction

An action that causes media playback to end.

Deprecated

enum EndAction

The actions that cause media playback to end.

Deprecated

