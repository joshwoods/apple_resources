

- MusicKit
- Playlist
-  Playlist.Kind 

Enumeration

# Playlist.Kind

The available kinds of playlists.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
enum Kind
```

## Topics

### Operators

static func == (Playlist.Kind, Playlist.Kind) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case editorial

Indicates that the playlist was created by an Apple Music curator.

case external

Indicates that the playlist was created by an external curator.

case personalMix

Indicates that the playlist is a personalized playlist for an Apple Music user.

case replay

Indicates that the playlist is a personalized Replay playlist for an Apple Music user.

case userShared

Indicates that the playlist was created and shared by an Apple Music user.

### Initializers

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func encode(to: any Encoder) throws

Encodes this value into the given encoder.

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Decodable
- Encodable
- Equatable
- Hashable
- Sendable

