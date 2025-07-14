

- AVFoundation
-  AVSampleCursorAudioDependencyInfo 

Structure

# AVSampleCursorAudioDependencyInfo

A structure that describes the independent decodability of audio samples.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct AVSampleCursorAudioDependencyInfo
```

## Topics

### Querying Independent Decodability

var audioSampleIsIndependentlyDecodable: ObjCBool

A Boolean value indicating whether the sample is independently decodable.

var audioSamplePacketRefreshCount: Int

The number of samples, starting at the current sample, that must be fed to the decoder to achieve full decoder refresh.

### Initializers

init()

Creates an audio sample decodability information structure.

init(audioSampleIsIndependentlyDecodable: ObjCBool, audioSamplePacketRefreshCount: Int)

Creates an audio sample decodability information structure with the specified values.

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

struct AVSampleCursorStorageRange

A structure that indicates the offset and length of storage for a media sample or its chunk.

struct AVSampleCursorChunkInfo

A value that provides information about a chunk of media samples.

