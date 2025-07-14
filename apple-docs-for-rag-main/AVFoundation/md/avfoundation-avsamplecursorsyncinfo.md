

- AVFoundation
-  AVSampleCursorSyncInfo 

Structure

# AVSampleCursorSyncInfo

A structure that describes the attributes of media samples to consider when resynchronizing a decoder.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct AVSampleCursorSyncInfo
```

## Topics

### Sync Information

var sampleIsFullSync: ObjCBool

A Boolean value that indicates whether a sample is a full sync sample.

var sampleIsPartialSync: ObjCBool

A Boolean value that indicates whether a sample is a partial sync sample.

var sampleIsDroppable: ObjCBool

A Boolean value that indicates whether a sample is droppable.

### Initializers

init()

Creates a sample cursor sync information structure.

init(sampleIsFullSync: ObjCBool, sampleIsPartialSync: ObjCBool, sampleIsDroppable: ObjCBool)

Creates a sample cursor sync information structure with media sample information.

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Sample cursors

class AVSampleCursor

An object that provides information about the media sample at the cursor’s current position.

struct AVSampleCursorDependencyInfo

A value for describing dependencies between a media sample and other media samples in the same sample sequence.

struct AVSampleCursorAudioDependencyInfo

A structure that describes the independent decodability of audio samples.

struct AVSampleCursorStorageRange

A structure that indicates the offset and length of storage for a media sample or its chunk.

struct AVSampleCursorChunkInfo

A value that provides information about a chunk of media samples.

