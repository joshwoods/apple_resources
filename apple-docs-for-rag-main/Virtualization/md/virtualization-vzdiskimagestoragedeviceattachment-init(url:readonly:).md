

- Virtualization
- VZDiskImageStorageDeviceAttachment
-  init(url:readOnly:) 

Initializer

# init(url:readOnly:)

Creates the attachment object from the specified disk image.

macOS 11.0+

``` source
init(
    url: URL,
    readOnly: Bool
) throws
```

## Parameters 

`url`  

A URL that points to a local disk image in RAW format.

`readOnly`  

A Boolean that indicates whether to configure the disk image as read-only. Specify true to prevent the guest operating system from writing to the disk image, and false to allow writing.

## Return Value

In Swift the methods returns an attachment object; in Objective-C the methods returns an attachment object on success, or `nil` if an error occurred

## See Also

### Creating the attachment point

init(url: URL, readOnly: Bool, cachingMode: VZDiskImageCachingMode, synchronizationMode: VZDiskImageSynchronizationMode) throws

Initialize the attachment from a local file URL.

