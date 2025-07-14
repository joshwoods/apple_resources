

- FSKit
-  FSBlockDeviceResource 

Class

# FSBlockDeviceResource

A resource that represents a block storage disk partition.

macOS 15.4+

``` source
class FSBlockDeviceResource
```

## Overview

A `FSBlockDeviceResource` can exist in either a proxied or nonproxied version. Only the `fskitd` daemon creates “real” (nonproxied) instances of this class. Client applications and daemons create proxy objects for requests, and `fskitd` opens the underlying device during the processing of the request.

This class wraps a file descriptor for a disk device or partition. Its fundamental identifier is the BSD disk name (bsdName) for the underlying IOMedia object. However, FSBlockDeviceResource doesn’t expose the underlying file descriptor. Instead, it provides accessor methods that can read from and write to the partition, either directly or using the kernel buffer cache.

When you use a `FSBlockDeviceResource`, your file system implementation also conforms to a maintenance operation protocol. These protocols add support for checking, repairing, and optionally formatting file systems. The system doesn’t mount block device file systems until they pass a file system check. For an FSUnaryFileSystem that uses `FSBlockDeviceResource`, conform to `FSManageableResourceMaintenanceOperations`.

## Topics

### Accessing resource properties

var bsdName: String

The device name of the resource.

var isWritable: Bool

A Boolean property that indicates whether the resource can write data to the device.

var blockCount: UInt64

The block count on this resource.

var blockSize: UInt64

The logical block size, the size of data blocks used by the file system.

var physicalBlockSize: UInt64

The sector size of the device.

### Reading and writing data

func read(into: UnsafeMutableRawBufferPointer, startingAt: off_t, length: Int) throws -> Int

Synchronously reads data from the resource into a buffer.

func read(into: UnsafeMutableRawBufferPointer, startingAt: off_t, length: Int) async throws -> Int

Asychronously reads data from the resource into a buffer.

func read(into: UnsafeMutableRawBufferPointer, startingAt: off_t, length: Int, completionHandler: (Int, (any Error)?) -> Void)

Reads data from the resource into a buffer and executes a closure afterwards.

func write(from: UnsafeRawBufferPointer, startingAt: off_t, length: Int) throws -> Int

Synchronously writes data from from a buffer to the resource and executes a block afterwards.

func write(from: UnsafeRawBufferPointer, startingAt: off_t, length: Int) async throws -> Int

Asynchronously writes data from from a buffer to the resource.

func write(from: UnsafeRawBufferPointer, startingAt: off_t, length: Int, completionHandler: (Int, (any Error)?) -> Void)

Writes data from from a buffer to the resource and executes a closure afterwards.

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

func metadataClear([FSMetadataRange], withDelayedWrites: Bool) throws

Clears the given ranges within the buffer cache.

func metadataPurge([FSMetadataRange]) throws

Synchronously purges the given ranges from the buffer cache.

class FSMetadataRange

A range that describes contiguous metadata segments on disk.

## Relationships

### Inherits From

- FSResource

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding

## See Also

### Resources

class FSResource

An abstract resource a file system uses to provide data for a volume.

