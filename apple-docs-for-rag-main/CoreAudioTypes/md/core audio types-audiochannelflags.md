

- Core Audio Types
-  AudioChannelFlags 

Structure

# AudioChannelFlags

Constants that define the audio channel flags of an audio channel description.

iOS 9.0+iPadOS 9.0+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
struct AudioChannelFlags
```

## Topics

### Flags

static var meters: AudioChannelFlags

A flag that indicates that unit values are in meters.

static var rectangularCoordinates: AudioChannelFlags

A flag that indicates the channel uses the speaker position’s cartesian coordinates.

static var sphericalCoordinates: AudioChannelFlags

A flag that indicates the channel uses the speaker position’s spherical coordinates.

### Initializers

init(rawValue: UInt32)

Creates a audio channel flags structure with a unsigned integer value.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Accessing the Data

var mChannelFlags: AudioChannelFlags

The audio channel flags that indicate how to interpret the channel coordinates.

var mChannelLabel: AudioChannelLabel

A label that describes the audio channel.

var mCoordinates: (Float32, Float32, Float32)

The coordinates that specify a precise speaker location.

typealias AudioChannelLabel

Identifies how an audio data channel is to be used.

Audio Channel Coordinates

Used in the `mChannelFlags` field of an AudioChannelDescription structure.

Audio Channel Labels

Channel labels for use in the `mChannelLabel` field of an AudioChannelDescription structure.

