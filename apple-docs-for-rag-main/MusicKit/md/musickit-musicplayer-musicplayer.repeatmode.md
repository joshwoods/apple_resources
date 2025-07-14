

- MusicKit
- MusicPlayer
-  MusicPlayer.RepeatMode 

Enumeration

# MusicPlayer.RepeatMode

The repeat modes for the music player.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 14.0+tvOS 15.0+visionOS 1.0+

``` source
enum RepeatMode
```

## Topics

### Operators

static func == (MusicPlayer.RepeatMode, MusicPlayer.RepeatMode) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case all

The music player is repeating the currently playing collection, such as an album or a playlist.

case none

The repeat mode is in a disabled state.

case one

The music player is repeating the currently playing entry.

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

- Copyable
- Equatable
- Hashable
- Sendable

