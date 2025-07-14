

- MediaExtension
-  MESampleLocation 

Class

# MESampleLocation

An object that provides information about the sample location with the media.

macOS 14.0+

``` source
class MESampleLocation
```

## Topics

### Creating a sample location

init(byteSource: MEByteSource, sampleLocation: AVSampleCursorStorageRange)

Creates a sample location object with the byte source and sample location that you specify.

### Inspecting a sample location

var byteSource: MEByteSource

The byte source to use to read the data for the sample.

var sampleLocation: AVSampleCursorStorageRange

The starting file offset and size in bytes of the sample.

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

class MESampleCursorChunk

An object that provides information about the chunk of media at the location of a sample.

class MEEstimatedSampleLocation

An object that provides information about the estimated sample location with the media.

class MEHEVCDependencyInfo

An object that provides information about the HEVC dependency attributes of a sample.

