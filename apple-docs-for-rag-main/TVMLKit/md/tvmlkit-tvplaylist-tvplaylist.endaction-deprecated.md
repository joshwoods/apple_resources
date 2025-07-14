

- TVMLKit
- TVPlaylist
-  TVPlaylist.EndAction Deprecated

Enumeration

# TVPlaylist.EndAction

The actions that cause media playback to end.

tvOS 12.0–18.0Deprecated

``` source
enum EndAction
```

Deprecated

Please use SwiftUI or UIKit

## Topics

### End Playback Reasons

case stop

The player has stopped playback

case pause

The player has paused playback.

case waitForMoreItems

The player is waiting for more media items.

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

enum RepeatMode

The modes that indicate how or whether media items can be replayed.

Deprecated

var endAction: TVPlaylist.EndAction

An action that causes media playback to end.

Deprecated

