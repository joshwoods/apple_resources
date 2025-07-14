

- MusicKit
- MusicPlayer
- MusicPlayer.Queue
-  MusicPlayer.Queue.EntryInsertionPosition 

Enumeration

# MusicPlayer.Queue.EntryInsertionPosition

An enumeration for the various supported positions for inserting playable music items or entries in the playback queue.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 14.0+tvOS 15.0+visionOS 1.0+

``` source
enum EntryInsertionPosition
```

## Topics

### Operators

static func == (MusicPlayer.Queue.EntryInsertionPosition, MusicPlayer.Queue.EntryInsertionPosition) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case afterCurrentEntry

A position that allows prepending entries in the playback queue, similar to the Play Next feature in the Music app.

case tail

A position that allows appending entries in the playback queue, similar to the Play Later feature in the Music app.

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

