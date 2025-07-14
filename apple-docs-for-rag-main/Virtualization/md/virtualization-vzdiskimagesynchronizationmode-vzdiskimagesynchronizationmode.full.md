

- Virtualization
- VZDiskImageSynchronizationMode
-  VZDiskImageSynchronizationMode.full 

Case

# VZDiskImageSynchronizationMode.full

Synchronizes data to the permanent storage holding the disk image.

macOS 12.0+

``` source
case full
```

## Discussion

This mode synchronizes the data with the permanent storage holding the disk image and ensures the data moves from the disk’s internal cache to permanent storage. This ensures there’s no loss of already synchronized data in the case of panic or loss of power.

## See Also

### Disk image synchronization modes

case fsync

Synchronizes data to the drive using the system’s best-effort synchronization mode.

case none

Disables data synchronization with the permanent storage.

