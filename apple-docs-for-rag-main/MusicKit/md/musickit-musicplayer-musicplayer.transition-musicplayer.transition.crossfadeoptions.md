

- MusicKit
- MusicPlayer
- MusicPlayer.Transition
-  MusicPlayer.Transition.CrossfadeOptions 

Structure

# MusicPlayer.Transition.CrossfadeOptions

The options for the crossfade transition.

iOS 18.0+iPadOS 18.0+

``` source
struct CrossfadeOptions
```

## Topics

### Operators

static func == (MusicPlayer.Transition.CrossfadeOptions, MusicPlayer.Transition.CrossfadeOptions) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Initializers

init(duration: TimeInterval?)

Creates options for a crossfade transition.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

CustomDebugStringConvertible Implementations

CustomStringConvertible Implementations

Equatable Implementations

## Relationships

### Conforms To

- Copyable
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- Sendable

