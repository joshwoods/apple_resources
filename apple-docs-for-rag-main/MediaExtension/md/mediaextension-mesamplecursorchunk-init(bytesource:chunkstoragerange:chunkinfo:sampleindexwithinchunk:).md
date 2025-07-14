

- MediaExtension
- MESampleCursorChunk
-  init(byteSource:chunkStorageRange:chunkInfo:sampleIndexWithinChunk:) 

Initializer

# init(byteSource:chunkStorageRange:chunkInfo:sampleIndexWithinChunk:)

Creates a new sample cursor chunk with byte source and chunk data that you provide.

macOS 14.0+

``` source
init(
    byteSource: MEByteSource,
    chunkStorageRange: AVSampleCursorStorageRange,
    chunkInfo: AVSampleCursorChunkInfo,
    sampleIndexWithinChunk: CFIndex
)
```

## Parameters 

`byteSource`  

The byte source to use to read the data for the sample.

`chunkStorageRange`  

The offset location and length of the sample’s chunk within the byte source.

`chunkInfo`  

An object that provides details about the chunk in the media.

`sampleIndexWithinChunk`  

The offset index of the sample within the chunk, in samples.

