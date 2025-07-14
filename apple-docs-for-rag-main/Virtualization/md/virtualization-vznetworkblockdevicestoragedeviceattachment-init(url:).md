

- Virtualization
- VZNetworkBlockDeviceStorageDeviceAttachment
-  init(url:) 

Initializer

# init(url:)

Creates a new network block device (NBD) storage attachment from an NDB Uniform Resource Indicator (URI) represented as a URL that you provide.

macOS 14.0+

``` source
convenience init(url URL: URL) throws
```

## Parameters 

`URL`  

The NBD’s URI represented as a URL.

## See Also

### Creating network block device attachments

init(url: URL, timeout: TimeInterval, isForcedReadOnly: Bool, synchronizationMode: VZDiskSynchronizationMode) throws

Creates a new network block device storage attachment from an NBD Uniform Resource Indicator (URI) represented as a URL, timeout value, and read-only and synchronization modes that you provide.

