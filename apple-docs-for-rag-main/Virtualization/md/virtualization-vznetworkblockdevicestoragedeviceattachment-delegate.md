

- Virtualization
- VZNetworkBlockDeviceStorageDeviceAttachment
-  delegate 

Instance Property

# delegate

The object that receives messages about changes to the network block device attachment.

macOS 14.0+

``` source
weak var delegate: (any VZNetworkBlockDeviceStorageDeviceAttachmentDelegate)? { get set }
```

## See Also

### Observing changes to the network block device

protocol VZNetworkBlockDeviceStorageDeviceAttachmentDelegate

Methods you implement to respond to changes to a network block device attachment.

