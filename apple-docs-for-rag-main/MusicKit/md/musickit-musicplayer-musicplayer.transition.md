

- MusicKit
- MusicPlayer
-  MusicPlayer.Transition 

Enumeration

# MusicPlayer.Transition

The transition applied between playing items.

iOS 18.0+iPadOS 18.0+

``` source
enum Transition
```

## Topics

### Structures

struct CrossfadeOptions

The options for the crossfade transition.

### Operators

static func == (MusicPlayer.Transition, MusicPlayer.Transition) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case crossfade(options: MusicPlayer.Transition.CrossfadeOptions)

A smooth overlap between the currently playing item and the next item.

case none

No transition.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Type Properties

static let crossfade: MusicPlayer.Transition

A smooth overlap between the currently playing item and the next item with default options.

### Type Methods

static func crossfade(duration: TimeInterval?) -> MusicPlayer.Transition

A smooth overlap between the currently playing item and the next item with a specified duration.

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

