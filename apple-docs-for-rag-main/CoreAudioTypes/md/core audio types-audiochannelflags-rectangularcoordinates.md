

- Core Audio Types
- AudioChannelFlags
-  rectangularCoordinates 

Type Property

# rectangularCoordinates

A flag that indicates the channel uses the speaker position’s cartesian coordinates.

iOS 2.0+iPadOS 2.0+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
static var rectangularCoordinates: AudioChannelFlags { get }
```

## Discussion

This flag is mutually exclusive with sphericalCoordinates.

## See Also

### Flags

static var meters: AudioChannelFlags

A flag that indicates that unit values are in meters.

static var sphericalCoordinates: AudioChannelFlags

A flag that indicates the channel uses the speaker position’s spherical coordinates.

