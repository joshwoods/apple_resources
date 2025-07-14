

- Virtualization
-  VZNetworkBlockDeviceStorageDeviceAttachmentDelegate 

Protocol

# VZNetworkBlockDeviceStorageDeviceAttachmentDelegate

Methods you implement to respond to changes to a network block device attachment.

macOS 14.0+

``` source
protocol VZNetworkBlockDeviceStorageDeviceAttachmentDelegate : NSObjectProtocol
```

## Topics

### Responding to connectivity changes

func attachment(VZNetworkBlockDeviceStorageDeviceAttachment, didEncounterError: any Error)

The method the attachment object calls when the NBD client encounters a nonrecoverable error.

func attachmentWasConnected(VZNetworkBlockDeviceStorageDeviceAttachment)

The method the attachment object calls when the NBD client successfully connects or reconnects with the server.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Observing changes to the network block device

var delegate: (any VZNetworkBlockDeviceStorageDeviceAttachmentDelegate)?

The object that receives messages about changes to the network block device attachment.

