

- FSKit
- FSVolume
-  FSVolume.PreallocateOperations 

Protocol

# FSVolume.PreallocateOperations

Methods and properties implemented by volumes that want to offer preallocation functions.

macOS 15.4+

``` source
protocol PreallocateOperations : NSObjectProtocol
```

## Overview

A preallocation operation allocates space for a file without writing to it yet. A file system may use reallocation to avoid performing space allocation while in the midst of I/O; this strategy improves performance. Also, if the expected I/O pattern is many small writes, preallocating contiguous chunks may prevent fragmenting the file system. This process can improve performance later.

In a kernel-based file system, you typically preallocate space with the `VNOP_ALLOCATE` operation, called from `fcntl(F_PREALLOCATE)`.

## Topics

### Preallocating space

func preallocateSpace(for: FSItem, at: off_t, length: Int, flags: FSVolume.PreallocateFlags, replyHandler: (Int, (any Error)?) -> Void)

Prealocates disk space for the given item.

**Required**

struct PreallocateFlags

Behavior flags for preallocation operations.

### Inspecting volume properties

var isPreallocateInhibited: Bool

A Boolean value that instructs FSKit not to call this protocol’s methods, even if the volume conforms to it.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Implementing optional operations

protocol OpenCloseOperations

Methods and properties implemented by volumes that want to receive open and close calls for each item.

protocol ReadWriteOperations

Methods implemented for read and write operations that deliver data to and from the extension.

protocol AccessCheckOperations

Methods and properties implemented by volumes that want to enforce access check operations.

protocol RenameOperations

Methods and properties implemented by volumes that support renaming the volume.

protocol FSVolumeKernelOffloadedIOOperations

Methods and properties implemented by volumes that use kernel-offloaded I/O to achieve higher file transfer performance.

protocol XattrOperations

Methods and properties implemented by volumes that natively or partially support extended attributes.

protocol ItemDeactivation

Methods and properties implemented by volumes that support deactivating items.

