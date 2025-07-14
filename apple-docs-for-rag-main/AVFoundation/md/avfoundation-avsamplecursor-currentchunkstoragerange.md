

- AVFoundation
- AVSampleCursor
-  currentChunkStorageRange 

Instance Property

# currentChunkStorageRange

The sample range in the storage container to load together with the current sample as a chunk.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 10.10+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var currentChunkStorageRange: AVSampleCursorStorageRange { get }
```

## Discussion

If the current chunk isn’t stored contiguously in its storage container, the property value’s offset is `-1`. In such cases use AVSampleBufferGenerator to obtain the sample data.

## See Also

### Getting Sample Information

var currentChunkInfo: AVSampleCursorChunkInfo

A value that provides information about the chunk of samples to which the current sample belongs.

struct AVSampleCursorChunkInfo

A value that provides information about a chunk of media samples.

struct AVSampleCursorStorageRange

A structure that indicates the offset and length of storage for a media sample or its chunk.

var currentChunkStorageURL: URL?

The URL of the storage container of the current sample and other samples to load in the same operation as a chunk.

var currentSampleDependencyInfo: AVSampleCursorDependencyInfo

The dependency information that describes relationships between a media sample and other media samples in the same sample sequence.

struct AVSampleCursorDependencyInfo

A value for describing dependencies between a media sample and other media samples in the same sample sequence.

var currentSampleDuration: CMTime

The decode duration of the sample at the cursor’s current position.

var currentSampleIndexInChunk: Int64

The index of the current sample within the chunk to which it belongs.

var currentSampleStorageRange: AVSampleCursorStorageRange

The offset and length of the current sample in the current chunk storage URL.

var currentSampleSyncInfo: AVSampleCursorSyncInfo

The synchronization information for the current sample for consideration when resynchronizing a decoder.

struct AVSampleCursorSyncInfo

A structure that describes the attributes of media samples to consider when resynchronizing a decoder.

func copyCurrentSampleFormatDescription() -> CMFormatDescription

Returns the format description of the sample at the cursor’s current position.

var currentSampleAudioDependencyInfo: AVSampleCursorAudioDependencyInfo

The independent decodability information for the audio sample.

var currentSampleDependencyAttachments: [AnyHashable : Any]?

A dictionary of dependency-related sample buffer attachments.

