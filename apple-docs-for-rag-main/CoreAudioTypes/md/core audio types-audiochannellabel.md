

- Core Audio Types
-  AudioChannelLabel 

Type Alias

# AudioChannelLabel

Identifies how an audio data channel is to be used.

iOS 2.0+iPadOS 2.0+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
typealias AudioChannelLabel = UInt32
```

## Discussion

This data type is used for the `mChannelLabel` field of the AudioChannelDescription structure. See Audio Channel Labels for possible values.

## See Also

### Accessing the Data

var mChannelFlags: AudioChannelFlags

The audio channel flags that indicate how to interpret the channel coordinates.

var mChannelLabel: AudioChannelLabel

A label that describes the audio channel.

var mCoordinates: (Float32, Float32, Float32)

The coordinates that specify a precise speaker location.

Audio Channel Coordinates

Used in the `mChannelFlags` field of an AudioChannelDescription structure.

struct AudioChannelFlags

Constants that define the audio channel flags of an audio channel description.

Audio Channel Labels

Channel labels for use in the `mChannelLabel` field of an AudioChannelDescription structure.

