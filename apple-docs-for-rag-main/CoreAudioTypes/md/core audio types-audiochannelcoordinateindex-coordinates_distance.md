

- Core Audio Types
- AudioChannelCoordinateIndex
-  coordinates_Distance 

Type Property

# coordinates_Distance

For spherical coordinates, distance is radially from the center. The units are specified by the `mChannelFlags` field of the `AudioChannelDescription` structure.

iOS 2.0+iPadOS 2.0+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
static var coordinates_Distance: AudioChannelCoordinateIndex { get }
```

## See Also

### Coordinates

enum AudioChannelCoordinateIndex

Indexes the fields of the `mCoordinates` array in an AudioChannelDescription structure.

static var coordinates_Azimuth: AudioChannelCoordinateIndex

For spherical coordinates, `0` is front center, positive is right, negative is left, and measurements are in degrees.

static var coordinates_Elevation: AudioChannelCoordinateIndex

For spherical coordinates, `+90` is zenith, `0` is horizontal, `-90` is nadir, and measurements are in degrees.

