

- Core Audio Types
- AudioChannelDescription
-  Audio Channel Coordinates 

API Collection

# Audio Channel Coordinates

Used in the `mChannelFlags` field of an AudioChannelDescription structure.

## Topics

### Coordinates

enum AudioChannelCoordinateIndex

Indexes the fields of the `mCoordinates` array in an AudioChannelDescription structure.

static var coordinates_Azimuth: AudioChannelCoordinateIndex

For spherical coordinates, `0` is front center, positive is right, negative is left, and measurements are in degrees.

static var coordinates_Distance: AudioChannelCoordinateIndex

For spherical coordinates, distance is radially from the center. The units are specified by the `mChannelFlags` field of the `AudioChannelDescription` structure.

static var coordinates_Elevation: AudioChannelCoordinateIndex

For spherical coordinates, `+90` is zenith, `0` is horizontal, `-90` is nadir, and measurements are in degrees.

### Flags

static var rectangularCoordinates: AudioChannelFlags

A flag that indicates the channel uses the speaker position’s cartesian coordinates.

static var sphericalCoordinates: AudioChannelFlags

A flag that indicates the channel uses the speaker position’s spherical coordinates.

static var meters: AudioChannelFlags

A flag that indicates that unit values are in meters.

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

struct AudioChannelFlags

Constants that define the audio channel flags of an audio channel description.

Audio Channel Labels

Channel labels for use in the `mChannelLabel` field of an AudioChannelDescription structure.

