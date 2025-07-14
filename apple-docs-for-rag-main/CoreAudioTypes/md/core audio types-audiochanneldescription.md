

- Core Audio Types
-  AudioChannelDescription 

Structure

# AudioChannelDescription

A structure that describes a channel of audio data.

iOS 2.0+iPadOS 2.0+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
struct AudioChannelDescription
```

## Topics

### Creating a Channel Description

init()

Creates an empty channel description.

init(mChannelLabel: AudioChannelLabel, mChannelFlags: AudioChannelFlags, mCoordinates: (Float32, Float32, Float32))

Creates a channel description with a label, flags, and coordinates.

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

struct AudioChannelFlags

Constants that define the audio channel flags of an audio channel description.

Audio Channel Labels

Channel labels for use in the `mChannelLabel` field of an AudioChannelDescription structure.

### Operators

static func == (AudioChannelDescription, AudioChannelDescription) -> Bool

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Channels

struct AudioChannelLayout

A structure that specifies a channel layout in a file or in hardware.

