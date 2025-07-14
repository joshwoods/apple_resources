

- Virtualization
- VZDiskImageStorageDeviceAttachment
-  init(url:readOnly:cachingMode:synchronizationMode:) 

Initializer

# init(url:readOnly:cachingMode:synchronizationMode:)

Initialize the attachment from a local file URL.

macOS 12.0+

``` source
init(
    url: URL,
    readOnly: Bool,
    cachingMode: VZDiskImageCachingMode,
    synchronizationMode: VZDiskImageSynchronizationMode
) throws
```

## Parameters 

`url`  

Local file URL to the disk image in RAW format.

`readOnly`  

If `true`, the device attachment is read-only, otherwise the device can write data to the disk image.

`cachingMode`  

The cacheing mode from one of the available VZDiskImageCachingMode options.

`synchronizationMode`  

How the disk image synchronizes with the underlying storage when the guest operating system flushes data, described by one of the available VZDiskImageSynchronizationMode modes.

## See Also

### Creating the attachment point

init(url: URL, readOnly: Bool) throws

Creates the attachment object from the specified disk image.

