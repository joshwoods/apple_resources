

- FSKit
- FSBlockDeviceResource
-  metadataFlush() 

Instance Method

# metadataFlush()

Synchronously flushes the resource’s buffer cache.

macOS 15.4+

``` source
func metadataFlush() throws
```

## Discussion

This method flushes data previously written with delayedMetadataWriteFrom:startingAt:length:error: to the resource.

## See Also

### Reading and writing data with kernel buffer cache

func metadataRead(into: UnsafeMutableRawBufferPointer, startingAt: off_t, length: Int) throws

Synchronously reads file system metadata from the resource into a buffer.

func metadataWrite(from: UnsafeRawBufferPointer, startingAt: off_t, length: Int) throws

Synchronously writes file system metadata from a buffer to the resource.

func delayedMetadataWrite(from: UnsafeRawBufferPointer, startingAt: off_t, length: Int) throws

Writes file system metadata from a buffer to a cache, prior to flushing it to the resource.

func asynchronousMetadataFlush() throws

Asynchronously flushes the resource’s buffer cache.

func metadataClear([FSMetadataRange], withDelayedWrites: Bool) throws

Clears the given ranges within the buffer cache.

func metadataPurge([FSMetadataRange]) throws

Synchronously purges the given ranges from the buffer cache.

class FSMetadataRange

A range that describes contiguous metadata segments on disk.

