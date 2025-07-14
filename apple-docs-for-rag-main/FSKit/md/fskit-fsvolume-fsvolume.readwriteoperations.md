

- FSKit
- FSVolume
-  FSVolume.ReadWriteOperations 

Protocol

# FSVolume.ReadWriteOperations

Methods implemented for read and write operations that deliver data to and from the extension.

macOS 15.4+

``` source
protocol ReadWriteOperations : NSObjectProtocol
```

## Overview

Most volumes conform to either this protocol or FSVolumeKernelOffloadedIOOperations. You can conform to both if you need to provide kernel-offloaded I/O only for certain files. In that case, files with the inhibitKernelOffloadedIO attribute set use this protocol, and those without it use FSVolumeKernelOffloadedIOOperations. A volume that doesn’t conform to either protocol can’t support any I/O operation.

## Topics

### Reading and writing

func read(from: FSItem, at: off_t, length: Int, into: FSMutableFileDataBuffer, replyHandler: (Int, (any Error)?) -> Void)

Reads the contents of the given file item.

**Required**

class FSMutableFileDataBuffer

A wrapper object for a data buffer.

func write(contents: Data, to: FSItem, at: off_t, replyHandler: (Int, (any Error)?) -> Void)

Writes contents to the given file item.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Implementing optional operations

protocol OpenCloseOperations

Methods and properties implemented by volumes that want to receive open and close calls for each item.

protocol AccessCheckOperations

Methods and properties implemented by volumes that want to enforce access check operations.

protocol RenameOperations

Methods and properties implemented by volumes that support renaming the volume.

protocol FSVolumeKernelOffloadedIOOperations

Methods and properties implemented by volumes that use kernel-offloaded I/O to achieve higher file transfer performance.

protocol PreallocateOperations

Methods and properties implemented by volumes that want to offer preallocation functions.

protocol XattrOperations

Methods and properties implemented by volumes that natively or partially support extended attributes.

protocol ItemDeactivation

Methods and properties implemented by volumes that support deactivating items.

