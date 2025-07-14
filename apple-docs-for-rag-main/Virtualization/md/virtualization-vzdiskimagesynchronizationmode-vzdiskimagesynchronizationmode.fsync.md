

- Virtualization
- VZDiskImageSynchronizationMode
-  VZDiskImageSynchronizationMode.fsync 

Case

# VZDiskImageSynchronizationMode.fsync

Synchronizes data to the drive using the system’s best-effort synchronization mode.

macOS 12.0+

``` source
case fsync
```

## Discussion

This mode synchronizes the data with the drive, but doesn’t ensure the data moves from the disk’s internal cache to permanent storage.

This is a best-effort mode with the same guarantees as the `fsync(_:)` system call.

## See Also

### Disk image synchronization modes

case full

Synchronizes data to the permanent storage holding the disk image.

case none

Disables data synchronization with the permanent storage.

