

- FSKit
- FSBlockDeviceResource
-  asynchronousMetadataFlush() 

Instance Method

# asynchronousMetadataFlush()

Asynchronously flushes the resource’s buffer cache.

macOS 15.4+

``` source
func asynchronousMetadataFlush() throws
```

## Discussion

This method schedules a flush of data previously written with delayedMetadataWriteFrom:startingAt:length:error: to the resource and returns immediately without blocking. This method doesn’t wait to check the flush’s status. If an error prevents the flush from being scheduled, the error is indicated by the in-out `error` parameter.

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

func metadataClear([FSMetadataRange], withDelayedWrites: Bool) throws

Clears the given ranges within the buffer cache.

func metadataPurge([FSMetadataRange]) throws

Synchronously purges the given ranges from the buffer cache.

class FSMetadataRange

A range that describes contiguous metadata segments on disk.

