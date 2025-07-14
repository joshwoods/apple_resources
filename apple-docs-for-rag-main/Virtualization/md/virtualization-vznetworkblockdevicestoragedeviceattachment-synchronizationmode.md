

- Virtualization
- VZNetworkBlockDeviceStorageDeviceAttachment
-  synchronizationMode 

Instance Property

# synchronizationMode

The mode in which the NBD client synchronizes data with the NBD server.

macOS 14.0+

``` source
var synchronizationMode: VZDiskSynchronizationMode { get }
```

## Discussion

See VZDiskSynchronizationMode for details on how the specific mode affects data synchronization between the NBD client and server.

## See Also

### Getting information about the attachment point

var isForcedReadOnly: Bool

Returns a Boolean value that indicates whether the underlying disk attachment network is in a read-only state.

var timeout: TimeInterval

The timeout value in seconds for the connection between the client and server.

var url: URL

The URL that refers to the NBD server to which the NBD client will connect.

