

- Core Audio Types
- AudioChannelDescription
-  mCoordinates 

Instance Property

# mCoordinates

The coordinates that specify a precise speaker location.

iOS 2.0+iPadOS 2.0+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
var mCoordinates: (Float32, Float32, Float32)
```

## Discussion

See AudioChannelCoordinateIndex for the interpretation of the items in the array.

## See Also

### Accessing the Data

var mChannelFlags: AudioChannelFlags

The audio channel flags that indicate how to interpret the channel coordinates.

var mChannelLabel: AudioChannelLabel

A label that describes the audio channel.

typealias AudioChannelLabel

Identifies how an audio data channel is to be used.

Audio Channel Coordinates

Used in the `mChannelFlags` field of an AudioChannelDescription structure.

struct AudioChannelFlags

Constants that define the audio channel flags of an audio channel description.

Audio Channel Labels

Channel labels for use in the `mChannelLabel` field of an AudioChannelDescription structure.

