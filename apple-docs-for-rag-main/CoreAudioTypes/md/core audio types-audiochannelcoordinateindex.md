

- Core Audio Types
-  AudioChannelCoordinateIndex 

Enumeration

# AudioChannelCoordinateIndex

Indexes the fields of the `mCoordinates` array in an AudioChannelDescription structure.

iOS 9.0+iPadOS 9.0+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
enum AudioChannelCoordinateIndex
```

## Topics

### Coordinates

case coordinates_BackFront

For rectangular coordinates, negative is back and positive is front. The units are specified by the `mChannelFlags` field.

case coordinates_DownUp

For rectangular coordinates, negative is below ground level, `0` is ground level, and positive is above ground level. The units are specified by the `mChannelFlags` field.

case coordinates_LeftRight

For rectangular coordinates, negative is left and positive is right. The units are specified by the `mChannelFlags` field of the `AudioChannelDescription` structure.

static var coordinates_Azimuth: AudioChannelCoordinateIndex

For spherical coordinates, `0` is front center, positive is right, negative is left, and measurements are in degrees.

static var coordinates_Distance: AudioChannelCoordinateIndex

For spherical coordinates, distance is radially from the center. The units are specified by the `mChannelFlags` field of the `AudioChannelDescription` structure.

static var coordinates_Elevation: AudioChannelCoordinateIndex

For spherical coordinates, `+90` is zenith, `0` is horizontal, `-90` is nadir, and measurements are in degrees.

### Initializers

init?(rawValue: UInt32)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Coordinates

static var coordinates_Azimuth: AudioChannelCoordinateIndex

For spherical coordinates, `0` is front center, positive is right, negative is left, and measurements are in degrees.

static var coordinates_Distance: AudioChannelCoordinateIndex

For spherical coordinates, distance is radially from the center. The units are specified by the `mChannelFlags` field of the `AudioChannelDescription` structure.

static var coordinates_Elevation: AudioChannelCoordinateIndex

For spherical coordinates, `+90` is zenith, `0` is horizontal, `-90` is nadir, and measurements are in degrees.

