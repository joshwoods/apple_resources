

- Virtualization
- VZDiskImageStorageDeviceAttachment
-  cachingMode 

Instance Property

# cachingMode

The current cacheing mode for the virtual disk image.

macOS 12.0+

``` source
var cachingMode: VZDiskImageCachingMode { get }
```

## See Also

### Getting the disk image details

var url: URL

The URL of the underlying disk image.

var isReadOnly: Bool

A Boolean value that indicates whether the underlying disk image is read-only.

var synchronizationMode: VZDiskImageSynchronizationMode

The mode in which the disk image synchronizes data with the underlying storage device.

