

- AVFoundation
- AVSampleCursorChunkInfo
-  init(chunkSampleCount:chunkHasUniformSampleSizes:chunkHasUniformSampleDurations:chunkHasUniformFormatDescriptions:) 

Initializer

# init(chunkSampleCount:chunkHasUniformSampleSizes:chunkHasUniformSampleDurations:chunkHasUniformFormatDescriptions:)

Creates a chunk information structure with the specified values.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
init(
    chunkSampleCount: Int64,
    chunkHasUniformSampleSizes: ObjCBool,
    chunkHasUniformSampleDurations: ObjCBool,
    chunkHasUniformFormatDescriptions: ObjCBool
)
```

## Parameters 

`chunkSampleCount`  

The count of media samples in the chunk.

`chunkHasUniformSampleSizes`  

The samples in the chunk occupy the same number of bytes in storage.

`chunkHasUniformSampleDurations`  

The samples in the chunk have the same duration.

`chunkHasUniformFormatDescriptions`  

The samples in the chunk have the same format description.

