

- Virtualization
- VZDiskBlockDeviceStorageDeviceAttachment
-  synchronizationMode 

Instance Property

# synchronizationMode

The value that defines how the disk synchronizes with the underlying storage when the guest operating system flushes data.

macOS 14.0+

``` source
var synchronizationMode: VZDiskSynchronizationMode { get }
```

## See Also

### Getting the block storage device details

var fileHandle: FileHandle

A file handle to a block device.

var isReadOnly: Bool

A Boolean value that indicates whether this disk attachment is read-only; otherwise, if the file handle allows writes, the device can write data into it.

