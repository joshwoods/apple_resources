

- MediaExtension
- MESampleCursorChunk
-  byteSource 

Instance Property

# byteSource

The byte source to use to read the data for the sample.

macOS 14.0+

``` source
var byteSource: MEByteSource { get }
```

## See Also

### Inspecting a chunk

var chunkStorageRange: AVSampleCursorStorageRange

The offset location and length of the sample’s chunk within the byte source.

var chunkInfo: AVSampleCursorChunkInfo

An object that provides details about the chunk in the media.

var sampleIndexWithinChunk: CFIndex

The offset index of the sample within the chunk, in samples.

