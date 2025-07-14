

- Virtualization
- VZDiskBlockDeviceStorageDeviceAttachment
-  isReadOnly 

Instance Property

# isReadOnly

A Boolean value that indicates whether this disk attachment is read-only; otherwise, if the file handle allows writes, the device can write data into it.

macOS 14.0+

``` source
var isReadOnly: Bool { get }
```

## See Also

### Getting the block storage device details

var fileHandle: FileHandle

A file handle to a block device.

var synchronizationMode: VZDiskSynchronizationMode

The value that defines how the disk synchronizes with the underlying storage when the guest operating system flushes data.

