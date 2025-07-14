

- MusicKit
- MusicPlayer
-  MusicPlayer.PlaybackStatus 

Enumeration

# MusicPlayer.PlaybackStatus

The music player playback status modes.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 14.0+tvOS 15.0+visionOS 1.0+

``` source
enum PlaybackStatus
```

## Overview

You determine a music player’s state by checking the playbackStatus property. Depending on the property’s value, you can update your app’s user interface or take other appropriate action.

## Topics

### Operators

static func == (MusicPlayer.PlaybackStatus, MusicPlayer.PlaybackStatus) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case interrupted

The music player is in an interrupted state, such as from an incoming phone call.

case paused

The music player is in a paused state.

case playing

The music player is playing.

case seekingBackward

The music player is seeking backward.

case seekingForward

The music player is seeking forward.

case stopped

The music player is in a stopped state.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable
- Hashable
- Sendable

