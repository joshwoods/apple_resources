

- FSKit
- FSBlockDeviceResource
-  metadataRead(into:startingAt:length:) 

Instance Method

# metadataRead(into:startingAt:length:)

Synchronously reads file system metadata from the resource into a buffer.

macOS 15.4+

``` source
func metadataRead(
    into buffer: UnsafeMutableRawBufferPointer,
    startingAt offset: off_t,
    length: Int
) throws
```

## Parameters 

`buffer`  

A buffer to receive the data.

`offset`  

The offset into the resource from which to start reading.

`length`  

The number of bytes to read.

## Discussion

This method provides access to the Kernel Buffer Cache, which is the primary system cache for file system metadata. Unlike equivalent kernel APIs, this method doesn’t hold any kernel-level claim to the underlying buffers.

For the read to succeed, requests must conform to any transfer requirements of the underlying resource. Disk drives typically require sector-addressed operations of one or more sector-aligned offsets, where a sector equals `physicalBlockSize`.

This method doesn’t support partial reading of metadata.

Throws

Any error encountered while reading data.

## See Also

### Reading and writing data with kernel buffer cache

func metadataWrite(from: UnsafeRawBufferPointer, startingAt: off_t, length: Int) throws

Synchronously writes file system metadata from a buffer to the resource.

func delayedMetadataWrite(from: UnsafeRawBufferPointer, startingAt: off_t, length: Int) throws

Writes file system metadata from a buffer to a cache, prior to flushing it to the resource.

func metadataFlush() throws

Synchronously flushes the resource’s buffer cache.

func asynchronousMetadataFlush() throws

Asynchronously flushes the resource’s buffer cache.

func metadataClear([FSMetadataRange], withDelayedWrites: Bool) throws

Clears the given ranges within the buffer cache.

func metadataPurge([FSMetadataRange]) throws

Synchronously purges the given ranges from the buffer cache.

class FSMetadataRange

A range that describes contiguous metadata segments on disk.

