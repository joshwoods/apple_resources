

- Virtualization
- VZDiskImageStorageDeviceAttachment
-  url 

Instance Property

# url

The URL of the underlying disk image.

macOS 11.0+

``` source
var url: URL { get }
```

## See Also

### Getting the disk image details

var isReadOnly: Bool

A Boolean value that indicates whether the underlying disk image is read-only.

var cachingMode: VZDiskImageCachingMode

The current cacheing mode for the virtual disk image.

var synchronizationMode: VZDiskImageSynchronizationMode

The mode in which the disk image synchronizes data with the underlying storage device.

