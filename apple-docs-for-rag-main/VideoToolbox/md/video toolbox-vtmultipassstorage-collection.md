

- Video Toolbox
-  VTMultiPassStorage 

API Collection

# VTMultiPassStorage

An object that stores video encoding metadata from a multipass encoding session.

## Topics

### Creating Storage Objects

func VTMultiPassStorageCreate(allocator: CFAllocator?, fileURL: CFURL?, timeRange: CMTimeRange, options: CFDictionary?, multiPassStorageOut: UnsafeMutablePointer&lt;VTMultiPassStorage?>) -> OSStatus

Creates a multipass storage object using a temporary file.

### Closing Storage Objects

func VTMultiPassStorageClose(VTMultiPassStorage) -> OSStatus

Ensures that any pending data is written to the multipass storage file and closes the file.

### Inspecting Storage Objects

func VTMultiPassStorageGetTypeID() -> CFTypeID

Retrieves the Core Foundation type identifier for the multipass storage object.

### Data Types

class VTMultiPassStorage

An object for storing information for each frame of a multipass compression session.

### Constants

let kVTMultiPassStorageCreationOption_DoNotDelete: CFString

Indicates that the multipass storage object’s backing store should not be deleted when finalized.

## See Also

### Compression

Encoding video for low-latency conferencing

Configure a compression session to optimize encoding for video-conferencing apps.

Encoding video for live streaming

Configure a compression session to encode video for live streaming.

Encoding video for offline transcoding

Configure a compression session to transcode video in offline workflows.

VTCompressionSession

An object that compresses video data.

VTDecompressionSession

An object that decompresses video data.

VTFrameSilo

An object that stores sample buffers from a multipass encoding session.

