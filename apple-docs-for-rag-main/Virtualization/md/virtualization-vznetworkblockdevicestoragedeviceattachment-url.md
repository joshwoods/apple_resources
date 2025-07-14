

- Virtualization
- VZNetworkBlockDeviceStorageDeviceAttachment
-  url 

Instance Property

# url

The URL that refers to the NBD server to which the NBD client will connect.

macOS 14.0+

``` source
var url: URL { get }
```

## See Also

### Getting information about the attachment point

var isForcedReadOnly: Bool

Returns a Boolean value that indicates whether the underlying disk attachment network is in a read-only state.

var synchronizationMode: VZDiskSynchronizationMode

The mode in which the NBD client synchronizes data with the NBD server.

var timeout: TimeInterval

The timeout value in seconds for the connection between the client and server.

