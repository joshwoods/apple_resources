

- MediaExtension
- MESampleCursorChunk
-  sampleIndexWithinChunk 

Instance Property

# sampleIndexWithinChunk

The offset index of the sample within the chunk, in samples.

macOS 14.0+

``` source
var sampleIndexWithinChunk: CFIndex { get }
```

## See Also

### Inspecting a chunk

var byteSource: MEByteSource

The byte source to use to read the data for the sample.

var chunkStorageRange: AVSampleCursorStorageRange

The offset location and length of the sample’s chunk within the byte source.

var chunkInfo: AVSampleCursorChunkInfo

An object that provides details about the chunk in the media.

