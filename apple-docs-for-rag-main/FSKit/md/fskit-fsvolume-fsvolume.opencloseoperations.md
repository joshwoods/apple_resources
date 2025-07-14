

- FSKit
- FSVolume
-  FSVolume.OpenCloseOperations 

Protocol

# FSVolume.OpenCloseOperations

Methods and properties implemented by volumes that want to receive open and close calls for each item.

macOS 15.4+

``` source
protocol OpenCloseOperations : NSObjectProtocol
```

## Overview

When a file system volume conforms to this protocol, the kernel layer issues an open call to indicate desired access, and a close call to indicate what access to retain. A file is fully closed when the kernel layer issues a close call with no retained open nodes. When a file system receives the close call, it removes all access to the item. When all memory mappings to the item release, the kernel layer issues a final close.

If a file system volume doesn’t conform to this protocol, the kernel layer can skip making such calls to the volume.

## Topics

### Opening and closing

func openItem(FSItem, modes: FSVolume.OpenModes, replyHandler: ((any Error)?) -> Void)

Opens a file for access.

**Required**

func closeItem(FSItem, modes: FSVolume.OpenModes, replyHandler: ((any Error)?) -> Void)

Closes a file from further access.

**Required**

struct OpenModes

Defined modes for opening a file.

### Inspecting volume properties

var isOpenCloseInhibited: Bool

A Boolean value that instructs FSKit not to call this protocol’s methods, even if the volume conforms to it.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Implementing optional operations

protocol ReadWriteOperations

Methods implemented for read and write operations that deliver data to and from the extension.

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

