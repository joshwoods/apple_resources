

- MusicKit
-  PlayParameters 

Structure

# PlayParameters

An opaque object that represents parameters to initiate playback of a playable music item using a music player.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct PlayParameters
```

## Topics

### Operators

static func == (PlayParameters, PlayParameters) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

Decodable Implementations

Encodable Implementations

Equatable Implementations

## Relationships

### Conforms To

- Copyable
- Decodable
- Encodable
- Equatable
- Hashable
- Sendable

## See Also

### Playback

class ApplicationMusicPlayer

An object your app uses to play music in a way that doesn’t affect the Music app’s state.

class SystemMusicPlayer

An object your app uses to play music by controlling the Music app’s state.

class MusicPlayer

An object your app uses to play music.

protocol PlayableMusicItem

A set of properties that a music player uses to initiate playback for a music item.

