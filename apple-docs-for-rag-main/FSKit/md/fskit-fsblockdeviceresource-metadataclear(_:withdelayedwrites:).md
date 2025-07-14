

- FSKit
- FSBlockDeviceResource
-  metadataClear(\_:withDelayedWrites:) 

Instance Method

# metadataClear(\_:withDelayedWrites:)

Clears the given ranges within the buffer cache.

macOS 15.4+

``` source
func metadataClear(
    _ rangesToClear: [FSMetadataRange],
    withDelayedWrites: Bool
) throws
```

## Parameters 

`rangesToClear`  

The metadata ranges to clear.

`withDelayedWrites`  

A Boolean value that determines whether to perform the clear operation with delayed writes. The delay works in the same manner as delayedMetadataWriteFrom:startingAt:length:error:. When using delayed writes, the client can flush the metadata with metadataFlush() or asynchronousMetadataFlush(). The system also flushes stale data in the buffer cache periodically.

## Discussion

This method clears the specified ranges in the resource’s buffer cache by writing zeroes into them.

## See Also

### Reading and writing data with kernel buffer cache

func metadataRead(into: UnsafeMutableRawBufferPointer, startingAt: off_t, length: Int) throws

Synchronously reads file system metadata from the resource into a buffer.

func metadataWrite(from: UnsafeRawBufferPointer, startingAt: off_t, length: Int) throws

Synchronously writes file system metadata from a buffer to the resource.

func delayedMetadataWrite(from: UnsafeRawBufferPointer, startingAt: off_t, length: Int) throws

Writes file system metadata from a buffer to a cache, prior to flushing it to the resource.

func metadataFlush() throws

Synchronously flushes the resource’s buffer cache.

func asynchronousMetadataFlush() throws

Asynchronously flushes the resource’s buffer cache.

func metadataPurge([FSMetadataRange]) throws

Synchronously purges the given ranges from the buffer cache.

class FSMetadataRange

A range that describes contiguous metadata segments on disk.

