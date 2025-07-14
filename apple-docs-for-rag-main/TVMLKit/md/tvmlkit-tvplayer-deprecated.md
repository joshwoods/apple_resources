

- TVMLKit
-  TVPlayer Deprecated

Class

# TVPlayer

A customizable native media player used to control playback from the JavaScript player used in an Apple TV client-server app.

tvOS 12.0–18.0Deprecated

``` source
class TVPlayer
```

Deprecated

Please use SwiftUI or UIKit

## Overview

You create a new `TVPlayer` object using your custom AVPlayer object. You can then play media items that are associated with the JavaScript media player using the new player. For example, you can add gestures, overlays, and other custom features to your TV player.

## Topics

### Setting Up the Player

init(player: AVPlayer)

Creates a new customizable player from an existing player.

var player: AVPlayer

The customizable media player.

var playlist: TVPlaylist?

The playlist for the media player.

### Controlling Playback

func next()

Plays the next media item in the playlist.

func pause()

Pauses the currently playing item.

func previous()

Plays the previous media item in the playlist.

var state: TVPlaybackState

The current state of the player.

enum TVPlaybackState

The possible states of a player.

func dispatch(event: TVPlaybackEvent, userInfo: (any TVPlaybackEventMarshaling)?, completion: ((Bool) -> Void)?)

Dispatches custom playback events to the JavaScript environment.

struct TVPlaybackEvent

Extend this structure to send your custom playback events to the JavaScript environment.

protocol TVPlaybackEventMarshaling

A protocol used for sending and receiving information across the JavaScript bridge.

class TVPlaybackCustomEventUserInfo

The user information used in a custom playback event.

### Inspecting Media Items

func setCurrentMediaItem(toItemAtIndex: Int)

Sets the current media item to the designated media item.

var previousMediaItem: TVMediaItem?

The previously selected media item.

var currentMediaItem: TVMediaItem?

The currently selected media item.

var nextMediaItem: TVMediaItem?

The next media item in the playlist.

### Instance Methods

func present(animated: Bool)

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

class TVPlaylist

A collection of media items associated with the Apple TV JavaScript player.

Deprecated

