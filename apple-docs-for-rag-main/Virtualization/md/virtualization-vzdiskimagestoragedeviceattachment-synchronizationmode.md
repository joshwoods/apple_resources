

- Virtualization
- VZDiskImageStorageDeviceAttachment
-  synchronizationMode 

Instance Property

# synchronizationMode

The mode in which the disk image synchronizes data with the underlying storage device.

macOS 12.0+

``` source
var synchronizationMode: VZDiskImageSynchronizationMode { get }
```

## See Also

### Getting the disk image details

var url: URL

The URL of the underlying disk image.

var isReadOnly: Bool

A Boolean value that indicates whether the underlying disk image is read-only.

var cachingMode: VZDiskImageCachingMode

The current cacheing mode for the virtual disk image.

