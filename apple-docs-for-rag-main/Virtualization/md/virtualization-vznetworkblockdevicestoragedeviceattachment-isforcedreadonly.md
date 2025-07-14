

- Virtualization
- VZNetworkBlockDeviceStorageDeviceAttachment
-  isForcedReadOnly 

Instance Property

# isForcedReadOnly

Returns a Boolean value that indicates whether the underlying disk attachment network is in a read-only state.

macOS 14.0+

``` source
var isForcedReadOnly: Bool { get }
```

## Discussion

The `forcedReadOnly` parameter affects how the Virtualization framework exposes the network block device (NBD) client to the guest operating system by the storage controller.

As part of the NBD protocol, during the handshake phase, the server advertises whether or not the disk the server exposes is read-only. Setting `forcedReadOnly` to true forces the NBD client to show up as read-only to the guest regardless of whether or not the NBD server advertises itself as read-only.

## See Also

### Getting information about the attachment point

var synchronizationMode: VZDiskSynchronizationMode

The mode in which the NBD client synchronizes data with the NBD server.

var timeout: TimeInterval

The timeout value in seconds for the connection between the client and server.

var url: URL

The URL that refers to the NBD server to which the NBD client will connect.

