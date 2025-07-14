

- MediaExtension
- MESampleCursorChunk
-  chunkStorageRange 

Instance Property

# chunkStorageRange

The offset location and length of the sample’s chunk within the byte source.

macOS 14.0+

``` source
var chunkStorageRange: AVSampleCursorStorageRange { get }
```

## See Also

### Inspecting a chunk

var byteSource: MEByteSource

The byte source to use to read the data for the sample.

var chunkInfo: AVSampleCursorChunkInfo

An object that provides details about the chunk in the media.

var sampleIndexWithinChunk: CFIndex

The offset index of the sample within the chunk, in samples.

