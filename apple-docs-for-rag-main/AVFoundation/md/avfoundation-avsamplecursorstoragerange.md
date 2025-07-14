

- AVFoundation
-  AVSampleCursorStorageRange 

Structure

# AVSampleCursorStorageRange

A structure that indicates the offset and length of storage for a media sample or its chunk.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct AVSampleCursorStorageRange
```

## Topics

### Storage Range

var offset: Int64

The offset of the first byte of storage that a media sample or its chunk occupies.

var length: Int64

The count of bytes of storage that a media sample or its chunk occupies.

### Initializers

init()

Creates a storage range structure.

init(offset: Int64, length: Int64)

Creates a storage range structure with offset and length values.

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Sample cursors

class AVSampleCursor

An object that provides information about the media sample at the cursor’s current position.

struct AVSampleCursorSyncInfo

A structure that describes the attributes of media samples to consider when resynchronizing a decoder.

struct AVSampleCursorDependencyInfo

A value for describing dependencies between a media sample and other media samples in the same sample sequence.

struct AVSampleCursorAudioDependencyInfo

A structure that describes the independent decodability of audio samples.

struct AVSampleCursorChunkInfo

A value that provides information about a chunk of media samples.

