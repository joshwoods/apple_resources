

- TVMLKit
-  TVPlaylist Deprecated

Class

# TVPlaylist

A collection of media items associated with the Apple TV JavaScript player.

tvOS 12.0–18.0Deprecated

``` source
class TVPlaylist
```

Deprecated

Please use SwiftUI or UIKit

## Overview

A `TVPlaylist` object contains read-only information about a playlist associated with the JavaScript player. You can use this information with your own custom AVPlayer objects exposed through a TVPlayer object. For example, you can retrieve album information from the JavaScript player and play the track through a `TVPlayer` object.

## Topics

### Retrieving Playlist Information

var mediaItems: [TVMediaItem]

An array of media items contained in the playlist.

var userInfo: [String : Any]?

User-defined metadata, like a developer-specific identifier, for a playlist.

var repeatMode: TVPlaylist.RepeatMode

A mode that determines how media items are replayed.

enum RepeatMode

The modes that indicate how or whether media items can be replayed.

var endAction: TVPlaylist.EndAction

An action that causes media playback to end.

enum EndAction

The actions that cause media playback to end.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Custom Player

class TVMediaItem

A single audio or video item associated with the Apple TV JavaScript player.

Deprecated

class TVPlayer

A customizable native media player used to control playback from the JavaScript player used in an Apple TV client-server app.

Deprecated

