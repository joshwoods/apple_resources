

- AVFoundation
-  AVSampleCursorDependencyInfo 

Structure

# AVSampleCursorDependencyInfo

A value for describing dependencies between a media sample and other media samples in the same sample sequence.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct AVSampleCursorDependencyInfo
```

## Topics

### Dependency Information

var sampleIndicatesWhetherItHasDependentSamples: ObjCBool

A Boolean value that determines whether the sample indicates if other samples depend on it.

var sampleHasDependentSamples: ObjCBool

A Boolean value that determines whether the sample has dependent samples.

var sampleIndicatesWhetherItDependsOnOthers: ObjCBool

A Boolean value that determines whether the sample indicates that it depends on other samples.

var sampleDependsOnOthers: ObjCBool

A Boolean value that determines whether the sample depends on other samples.

var sampleIndicatesWhetherItHasRedundantCoding: ObjCBool

A Boolean value that determines whether the sample indicates that it has redundant coding.

var sampleHasRedundantCoding: ObjCBool

A Boolean value that determines whether the sample has redundant coding.

### Initializers

init()

Creates a sample cursor dependency information structure.

init(sampleIndicatesWhetherItHasDependentSamples: ObjCBool, sampleHasDependentSamples: ObjCBool, sampleIndicatesWhetherItDependsOnOthers: ObjCBool, sampleDependsOnOthers: ObjCBool, sampleIndicatesWhetherItHasRedundantCoding: ObjCBool, sampleHasRedundantCoding: ObjCBool)

Creates a sample cursor dependency information structure with sample information.

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

struct AVSampleCursorAudioDependencyInfo

A structure that describes the independent decodability of audio samples.

struct AVSampleCursorStorageRange

A structure that indicates the offset and length of storage for a media sample or its chunk.

struct AVSampleCursorChunkInfo

A value that provides information about a chunk of media samples.

