

- Virtualization
- VZDiskImageStorageDeviceAttachment
-  isReadOnly 

Instance Property

# isReadOnly

A Boolean value that indicates whether the underlying disk image is read-only.

macOS 11.0+

``` source
var isReadOnly: Bool { get }
```

## Discussion

If the value of this property is true, the guest operating system may read the contents of the disk image, but may not write to it.

## See Also

### Getting the disk image details

var url: URL

The URL of the underlying disk image.

var cachingMode: VZDiskImageCachingMode

The current cacheing mode for the virtual disk image.

var synchronizationMode: VZDiskImageSynchronizationMode

The mode in which the disk image synchronizes data with the underlying storage device.

