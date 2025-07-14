

- Core Media I/O
-  CMIOExtensionStreamFormat 

Class

# CMIOExtensionStreamFormat

An object that describes the format of a media stream.

Mac Catalyst 15.4+macOS 12.3+

``` source
class CMIOExtensionStreamFormat
```

## Topics

### Creating a Stream Format

convenience init(formatDescription: CMFormatDescription, maxFrameDuration: CMTime, minFrameDuration: CMTime, validFrameDurations: [CMTime]?)

Creates a stream format with a format description and frame durations.

### Configuring Frame Durations

var minFrameDuration: CMTime

The minimum frame duration a stream supports.

var maxFrameDuration: CMTime

The maximum duration a stream supports.

var validFrameDurations: [CMTime]?

An array of frame durations the stream supports.

### Accessing the Format Description

var formatDescription: CMFormatDescription

A description of the format of the stream’s media samples.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Accessing the Source Format

var formats: [CMIOExtensionStreamFormat]

An array of formats that a stream supports.

**Required**

