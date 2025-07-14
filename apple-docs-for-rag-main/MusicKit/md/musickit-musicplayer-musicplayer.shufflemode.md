

- MusicKit
- MusicPlayer
-  MusicPlayer.ShuffleMode 

Enumeration

# MusicPlayer.ShuffleMode

The shuffle modes for the music player.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 14.0+tvOS 15.0+visionOS 1.0+

``` source
enum ShuffleMode
```

## Topics

### Operators

static func == (MusicPlayer.ShuffleMode, MusicPlayer.ShuffleMode) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case off

The shuffle mode is in a disabled state.

case songs

The music player’s shuffle songs mode.

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

