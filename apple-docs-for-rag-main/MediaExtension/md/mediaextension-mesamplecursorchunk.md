

- MediaExtension
-  MESampleCursorChunk 

Class

# MESampleCursorChunk

An object that provides information about the chunk of media at the location of a sample.

macOS 14.0+

``` source
class MESampleCursorChunk
```

## Overview

The chunkDetails() method returns an instance of this class.

## Topics

### Creating a sample cursor chunk

init(byteSource: MEByteSource, chunkStorageRange: AVSampleCursorStorageRange, chunkInfo: AVSampleCursorChunkInfo, sampleIndexWithinChunk: CFIndex)

Creates a new sample cursor chunk with byte source and chunk data that you provide.

### Inspecting a chunk

var byteSource: MEByteSource

The byte source to use to read the data for the sample.

var chunkStorageRange: AVSampleCursorStorageRange

The offset location and length of the sample’s chunk within the byte source.

var chunkInfo: AVSampleCursorChunkInfo

An object that provides details about the chunk in the media.

var sampleIndexWithinChunk: CFIndex

The offset index of the sample within the chunk, in samples.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol
- Sendable

## See Also

### Sample cursors

protocol MESampleCursor

A protocol that defines the information to provide about samples within a track of a media asset, and enables stepping through samples in the track in decode or presentation order.

class MESampleLocation

An object that provides information about the sample location with the media.

class MEEstimatedSampleLocation

An object that provides information about the estimated sample location with the media.

class MEHEVCDependencyInfo

An object that provides information about the HEVC dependency attributes of a sample.

