

- AVFoundation
-  AVSampleCursorChunkInfo 

Structure

# AVSampleCursorChunkInfo

A value that provides information about a chunk of media samples.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct AVSampleCursorChunkInfo
```

## Topics

### Chunk Information

var chunkSampleCount: Int64

The count of media samples in the chunk.

var chunkHasUniformSampleSizes: ObjCBool

The samples in the chunk occupy the same number of bytes in storage.

var chunkHasUniformSampleDurations: ObjCBool

The samples in the chunk have the same duration.

var chunkHasUniformFormatDescriptions: ObjCBool

The samples in the chunk have the same format description.

### Initializers

init()

Creates a chunk information structure.

init(chunkSampleCount: Int64, chunkHasUniformSampleSizes: ObjCBool, chunkHasUniformSampleDurations: ObjCBool, chunkHasUniformFormatDescriptions: ObjCBool)

Creates a chunk information structure with the specified values.

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

struct AVSampleCursorStorageRange

A structure that indicates the offset and length of storage for a media sample or its chunk.

