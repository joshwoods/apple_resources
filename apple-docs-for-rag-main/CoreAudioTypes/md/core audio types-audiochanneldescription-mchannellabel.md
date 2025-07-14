

- Core Audio Types
- AudioChannelDescription
-  mChannelLabel 

Instance Property

# mChannelLabel

A label that describes the audio channel.

iOS 2.0+iPadOS 2.0+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
var mChannelLabel: AudioChannelLabel
```

## See Also

### Accessing the Data

var mChannelFlags: AudioChannelFlags

The audio channel flags that indicate how to interpret the channel coordinates.

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

