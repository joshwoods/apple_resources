

- MediaExtension
-  MEHEVCDependencyInfo 

Class

# MEHEVCDependencyInfo

An object that provides information about the HEVC dependency attributes of a sample.

macOS 14.0+

``` source
class MEHEVCDependencyInfo
```

## Topics

### Inspecting the HEVC dependency attributes of a sample

var hasTemporalSubLayerAccess: Bool

A Boolean value that indicates if the sample has an HEVC temporal sublayer access (TSA) picture.

var hasStepwiseTemporalSubLayerAccess: Bool

A Boolean value that indicates if the sample has an HEVC stepwise temporal sublayer access (STSA) picture.

var syncSampleNALUnitType: Int16

The NAL unit type for HEVC sync sample groups.

var temporalLevel: Int16

The HEVC temporal level, if available.

var profileSpace: Int16

The HEVC profile space, if available.

var tierFlag: Int16

The HEVC tier level flag, if available.

var profileIndex: Int16

The HEVC profile index, if available.

var profileCompatibilityFlags: Data?

The HEVC profile compatibility flags (4 bytes), if available.

var constraintIndicatorFlags: Data?

The HEVC constraint indicator flags (6 bytes), if available.

var levelIndex: Int16

The HEVC level index, if available.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol
- Sendable

## See Also

### Sample cursors

protocol MESampleCursor

A protocol that defines the information to provide about samples within a track of a media asset, and enables stepping through samples in the track in decode or presentation order.

class MESampleLocation

An object that provides information about the sample location with the media.

class MESampleCursorChunk

An object that provides information about the chunk of media at the location of a sample.

class MEEstimatedSampleLocation

An object that provides information about the estimated sample location with the media.

