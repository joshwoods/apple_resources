

- MusicKit
-  AudioVariant 

Enumeration

# AudioVariant

Variants that indicate the quality of audio available for an item.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
enum AudioVariant
```

## Topics

### Operators

static func == (AudioVariant, AudioVariant) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case dolbyAtmos

Dolby Atmos is an immersive audio experience that surrounds you with sound from all sides, including above.

case dolbyAudio

Dolby Audio is a surround sound format that includes Dolby 5.1 and 7.1.

case highResolutionLossless

Hi-Res Lossless uses Apple Lossless Audio Codec (ALAC) for bit-for-bit accuracy up to 24-bit/192 kHz.

case lossless

Lossless uses Apple Lossless Audio Codec (ALAC) for bit-for-bit accuracy up to 24-bit/48 kHz.

case lossyStereo

Lossy stereo uses compression used to store sound data.

case spatialAudio

Spatial audio is a fallback mode if the content is Dolby Atmos or Dolby Audio, but hardware capabilities don’t support them.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Type Aliases

typealias AllCases

A type that can represent a collection of all values of this type.

### Type Properties

static var allCases: [AudioVariant]

A collection of all values of this type.

### Default Implementations

CustomStringConvertible Implementations

Decodable Implementations

Encodable Implementations

Equatable Implementations

## Relationships

### Conforms To

- CaseIterable
- Copyable
- CustomStringConvertible
- Decodable
- Encodable
- Equatable
- Hashable
- Sendable

