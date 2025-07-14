

- Virtualization
- VZDiskBlockDeviceStorageDeviceAttachment
-  fileHandle 

Instance Property

# fileHandle

A file handle to a block device.

macOS 14.0+

``` source
var fileHandle: FileHandle { get }
```

## See Also

### Getting the block storage device details

var isReadOnly: Bool

A Boolean value that indicates whether this disk attachment is read-only; otherwise, if the file handle allows writes, the device can write data into it.

var synchronizationMode: VZDiskSynchronizationMode

The value that defines how the disk synchronizes with the underlying storage when the guest operating system flushes data.

