

- MediaExtension
- MESampleCursorChunk
-  chunkInfo 

Instance Property

# chunkInfo

An object that provides details about the chunk in the media.

macOS 14.0+

``` source
var chunkInfo: AVSampleCursorChunkInfo { get }
```

## See Also

### Inspecting a chunk

var byteSource: MEByteSource

The byte source to use to read the data for the sample.

var chunkStorageRange: AVSampleCursorStorageRange

The offset location and length of the sample’s chunk within the byte source.

var sampleIndexWithinChunk: CFIndex

The offset index of the sample within the chunk, in samples.

