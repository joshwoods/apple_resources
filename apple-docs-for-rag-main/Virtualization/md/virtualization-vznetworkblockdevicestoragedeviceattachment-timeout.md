

- Virtualization
- VZNetworkBlockDeviceStorageDeviceAttachment
-  timeout 

Instance Property

# timeout

The timeout value in seconds for the connection between the client and server.

macOS 14.0+

``` source
var timeout: TimeInterval { get }
```

## Discussion

When the timeout expires, the client attempts to reconnect with the server. If after several retries, the client can’t reestablish a connection to the server, the framework invokes the attachment(_:didEncounterError:) delegate method.

## See Also

### Getting information about the attachment point

var isForcedReadOnly: Bool

Returns a Boolean value that indicates whether the underlying disk attachment network is in a read-only state.

var synchronizationMode: VZDiskSynchronizationMode

The mode in which the NBD client synchronizes data with the NBD server.

var url: URL

The URL that refers to the NBD server to which the NBD client will connect.

