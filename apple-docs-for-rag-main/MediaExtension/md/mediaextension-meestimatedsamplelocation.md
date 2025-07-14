

- MediaExtension
-  MEEstimatedSampleLocation 

Class

# MEEstimatedSampleLocation

An object that provides information about the estimated sample location with the media.

macOS 14.0+

``` source
class MEEstimatedSampleLocation
```

## Topics

### Creating an estimated sample location

init(byteSource: MEByteSource, estimatedSampleLocation: AVSampleCursorStorageRange, refinementDataLocation: AVSampleCursorStorageRange)

Creates an estimated sample location object with the byte source, sample location, and data location that you specify.

### Inspecting an estimated sample location

var byteSource: MEByteSource

The byte source to use to read the data for the sample.

var estimatedSampleLocation: AVSampleCursorStorageRange

The estimated starting file offset and size in bytes of the sample.

var refinementDataLocation: AVSampleCursorStorageRange

The starting file offset and size in bytes of the data necessary to provide an accurate sample location.

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

class MEHEVCDependencyInfo

An object that provides information about the HEVC dependency attributes of a sample.

